# Introduction

Iceburg CRM is a metadriven CRM that allows you to quickly prototype any CRM.  The default CRM is based on a typical business CRM but the flexibility of dymanic modules, fields, subpanels allows prototyping of any number of different tyes of CRMs.    

Iceburg CRM is created with:

- [Vue 3](https://vuejs.org/) for the frontend
- [Laravel 9](https://laravel.com/) for the backend
- [Tailwind CSS](https://tailwindcss.com/) with the [daisyUI](https://daisyui.com/) plugin
- [Inertia](https://inertiajs.com/) for routing
- [heroicons](https://heroicons.com)

## Features

- Meta Driven CRM 
- Dymanic Modules, Fields, Relationships, Subpanels
- Unlimited Relationships
- Importing / Exporting
- Convertable Modules

## License

[MIT](https://opensource.org/licenses/MIT)

## Modules

Modules represent database tables.

### Import / Export

Importing and Exporting is based on [Larave-Excel](https://laravel-excel.com/) and supports 6 different types of files

- XLSX
- CSV
- TSV
- ODS
- XLS
- HTML


Importing data into a module will automatically convert related data into related module ids based on the module you are importing into.

For example if you had a related field of Countries and you input a file with a country name like 'Canada' the system will find the related country module  record and convert 'Canada' to 2 (or whatever the related id is defined as).

### Convert To (Modules_Convertables)

A convertto record allow a module to relate to another module and have a record be used to seed another table.  

An example would be a lead could be converted to a contact, account, or opportunity.  Whatever fields are in common will populate with the information present in the origating table.

The Module_Convertables is the table that holds this information

## Fields

Fields represent database columns for tables

## Relationship

Relationships are the container that holds definition and data connecting 2 or more modules.

Relationships are implicit and modules do not need to contain fields that relate to each other.  The relationship record and related tables will hold the definition of the modules 

You can create relationship with an <b>unlimited</b> number of modules.  

The relationship table has a relationship to relationship_modules which contains the relationships modules.  

## Subpanels

Are a specific view with fields for a relationship.

A subpanel is attached to a module record.

Module_Subpanel table has a relationship to subpanel_fields which defines the fields for the subpanel.

The same relationships can be reused in different subpanels.  This allows related data in the relationship to be available in different places.


## Datalets

Datalets are dashboard components used for displaying information on a graphical manner.