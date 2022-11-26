# Seeding

This section allows you to define and seed your CRM.  The ordering of the seeder files are important because many objects rely on the existance of other data elements to be created.

The default CRM contains faker data.  This was be removed from either setting the faker_seeder field to 0 on the module object or by changing the value of the number of seed in the generate seeder file.


## Module Seeder

The module seeder class holds the module definitions

```php
Module::insert([
            'name' => 'datalets',
            'label' => 'Datalets',
            'description' => 'System Datalets',
            'view_order' => $order++,
            'module_group_id' => 6,
            'faker_seed' => 0,
            'create_table' => 0,
            'admin' => 1,
            'status' => 1
        ]);
```

## Field Seeder

The field seeder class holds the field definitions and contains the name of the module in the method name.

```php
$order=0;
        $moduleId=Module::getId(__FUNCTION__);

        Field::insert(Field::getField([
            'name'          => 'test_color',
            'label'         => 'color',
            'module_id'     => $moduleId,
            'input_type'    => 'color',
            'field_length'  => 10,
        ], $order++));
```


## Relationship Seeder

The relationship seeder holds the relationship definitions.  The name of the table can be anything but we suggest putting the name of the tables in order with an underscore separating them.

```php
Relationship::insert([
            'name' => 'documents_users',
            'modules' => implode(",", [
                Module::where('name', 'documents')->first()->id,
                Module::where('name', 'users')->first()->id,
            ]),
            'related_field_types' => 'integer,integer',
        ]);
```

## Generate Seeder

This is the file that generates the modules, fields, relationships, users and seeds the data.  It also generates a workflow table, datalets and other data related tables.  The name of the function must match the name of the table.


## Module Subpanel Seeder

This is the file that generates the subpanels.  A ModuleSubpanel and SubpanelFields are created and linked

```php
$id=ModuleSubpanel::insertGetId([
            'name' => 'accounts_contacts',
            'label' => 'Contacts',
            'relationship_id' => Relationship::where('name', 'accounts_contacts')
                ->orWhere('name', 'contacts_accounts')->first()->id,
            'module_id' => Module::where('name', 'accounts')->first()->id,
        ]);
        SubpanelField::insert([
            'subpanel_id' => $id,
            'field_id' => Field::where('module_id',
                Module::where('name', 'contacts')->first()->id
            )
                ->where('name', 'first_name')->first()->id
        ]);
        SubpanelField::insert([
            'subpanel_id' => $id,
            'field_id' => Field::where('module_id',
                Module::where('name', 'contacts')->first()->id
            )
                ->where('name', 'last_name')->first()->id
        ]);
```



## Generate Subpanels

This file generated the subpanels and data.  
