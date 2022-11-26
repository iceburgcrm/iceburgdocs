# Administration

## Settings

Settings are available to anyone with the 'Admin' role.  

1. Change Site Title
2. Change Site Description
3. Change Theme
4. Default Number of Search Results
5. Default Number of Search Results for Subpanels
6. Maximum Number of Records to be Exported

### Theme

Themes are based on [Daisyui](https://daisyui.com/docs/themes/) theming system.  But default 26 different themes are available and you have the ability to create your own theme or customize an existing theme.  Each theme has a color schema for primary, secondary and accent colors.  Light and dark themes are available. 

## Permissions

There are two types of permissions.  General permissions and admin permissions.  

### Admin Permissions

Any admin module or admin section requires the user to have the 'Admin' role.  
 
### General Permissions

You can set permissions based on module for different roles.

The permission types are
1. Read
2. Write
3. Import
4. Export

## Adding a new User

To add a new user go to the admin module and add a new record.  The signup registration is disabled by default but could be renamed by removed commented out signup routes.

## Module Settings

Modules settings can be changed in the module settings section.  

- name               - Name of the database column
- label 			  - Display Name
- description		  - Description of the module
- status			  - Active or Disabled
- faker_seeder       - Used to determined if seeding is required
- create_table		  - Used to determine if generating the table is necessary
- view_order		  - Order used for display 
- admin  			  - Is this module an Admin module (only admin users can access these modules)
- parent_id		  - Used to determine is a parent module exists
- icon              - Name of the [heroicon](https://heroicons.com).  Needs to be defined in the BaseIcon vue file
- module_group_id   - ID of the module group which is used for the top menu display


## Field Settings

- name               - Name of the database column
- label 			  - Display Name
- module_id		  - Module_ID the field belongs to
- validation		  - Laravel rules syntax
- input_type         - The type of field
- data_type          - The column type used for generation
- field_length       - The length of the field used for generation
- is_nullable        - Does the column allow nulls
- related_module_id - The module_id of the related table
- related_field_id  - The id of the field record for the related table
- related_value_id  - The name of the column 
- decimal_places    - Number of decimal places used for generation
- status            - Is the field active

### Validation

Validation uses [Laravel](https://laravel.com/docs/9.x/validation#available-validation-rules) based validation rules and syntax.

```php
'required:max:100'
```

### Input Types

Iceburg CRM support's these fields:

- 'currency'
- 'checkbox'
- 'color'
- 'date',
- 'email'
- 'number'
- 'password'
-  'tel', 
- 'text', 
- 'url', 
- textarea', 
- 'city', 
- 'zip', 
- 'address', 
- 'related'



#### Related

Related modules represent a relationship from a single field to another module record value.

Related fields can be defined by setting:
input_type        - 'related'
related_module_id - The module_id of the related table
related_field_id  - The id of the field record for the related table
related_value_id  - The name of the column 

## Relationship Settings

A relationship, connected to the relationship_modules table holds the information on how to define a relationship.


- name                - Database table name
- related_field_types - The datatypes of the connecting relationship
- status              - Active or Disabled



## Subpanel Settings

The Module_Subpanel module allows you to change these values:
- name               - This is the name of the table.  Changing this for an active value without regenerating will cause errors
- label              - The display name
- module_id          - The base module_id the subpanel is linked to
- list_size	      - Size of the list, this will get overridden by the default subpanel value
- list_order_column  - Search order of the subpanel
- list_order	      - Order direction
- relationship_id    - ID of the relationship the subpanel is connected to
- status             - Is the Subpanel active or disabled
- modules			  - This is used for defining modules for seeding

## Datalet Settings 

Datalets current use these values:

- Label 		 - Title of Graph
- Type  		 - Which is a related key to the datalet_types table/module
- Display_order - The order the datalets are displayed
- Active        - This field allows you to disable the datalet 