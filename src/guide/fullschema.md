# Full Schema

## Tables / Fields


### account_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts
| Field name | Type |
| --- | --- |
| test_color | varchar(255) | 
| test_checkbox | tinyint(1) | 
| name | varchar(255) | 
| first_name | varchar(255) | 
| last_name | varchar(255) | 
| email | varchar(255) | 
| phone | varchar(255) | 
| fax | varchar(255) | 
| website | varchar(255) | 
| address | varchar(255) | 
| city | varchar(255) | 
| zip | varchar(255) | 
| state | int(11) | 
| country | int(11) | 
| description | varchar(255) | 
| status | int(11) | 
| assigned_to | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts_cases
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| cases_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts_contacts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| contacts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts_contracts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| contracts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts_invoices
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| invoices_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts_invoices_users
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| invoices_id | int(10) unsigned | 
| users_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts_meetings
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| meetings_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### accounts_opportunities
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| opportunities_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### campaign_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### campaign_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### campaigns
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| status | int(11) | 
| budget | double | 
| forecast | double | 
| actual | double | 
| impressions | int(11) | 
| currency | int(11) | 
| campaign_type | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### campaigns_accounts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| campaigns_id | int(10) unsigned | 
| accounts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### campaigns_tasks
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| campaigns_id | int(10) unsigned | 
| tasks_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### case_priorities
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### case_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### case_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### cases
| Field name | Type |
| --- | --- |
| subject | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| case_number | int(11) | 
| status | int(11) | 
| priority | int(11) | 
| type | int(11) | 
| resolution | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### contacts
| Field name | Type |
| --- | --- |
| first_name | varchar(255) | 
| last_name | varchar(255) | 
| email | varchar(255) | 
| phone | varchar(255) | 
| fax | varchar(255) | 
| website | varchar(255) | 
| address | varchar(255) | 
| city | varchar(255) | 
| state | int(11) | 
| zip | varchar(255) | 
| country | int(11) | 
| description | varchar(255) | 
| status | int(11) | 
| email_receive | tinyint(1) | 
| assigned_to | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### contract_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### contract_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### contracts
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| discount | double | 
| taxes | double | 
| shipping | double | 
| subtotal | double | 
| total | double | 
| currency | int(11) | 
| signed_by | int(11) | 
| assigned_to | int(11) | 
| contract_type | int(11) | 
| start_date | int(11) | 
| end_date | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### contracts_lineitems
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| contracts_id | int(10) unsigned | 
| lineitems_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### countries
| Field name | Type |
| --- | --- |
| code | varchar(255) | 
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### currency
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| code | varchar(255) | 
| symbol | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### datalet_types
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(255) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### datalets
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(255) | 
| label | varchar(255) | 
| type | int(11) | 
| role_id | int(11) | 
| field_id | int(11) | 
| module_id | int(11) | 
| relationship_id | int(11) | 
| size | int(11) | 
| display_order | int(11) | 
| active | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### discount_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### document_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### document_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| file_link | varchar(255) | 
| document_type | int(11) | 
| document_status | int(11) | 
| expire_date | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents_accounts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| accounts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents_cases
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| cases_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents_contracts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| contracts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents_meetings
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| meetings_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents_opportunities
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| opportunities_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents_tasks
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| tasks_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### documents_users
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| users_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### failed_jobs
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| uuid | varchar(255) | 
| connection | text | 
| queue | text | 
| payload | longtext | 
| exception | longtext | 
| failed_at | timestamp | 


### fields
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| label | varchar(255) | 
| module_id | int(11) | 
| validation | varchar(255) | 
| input_type | varchar(255) | 
| data_type | varchar(100) | 
| field_length | int(11) | 
| required | int(11) | 
| is_nullable | tinyint(4) | 
| default_value | varchar(255) | 
| read_only | tinyint(4) | 
| disabled | tinyint(4) | 
| related_module_id | int(11) | 
| related_field_id | varchar(255) | 
| related_value_id | varchar(255) | 
| decimal_places | int(11) | 
| status | tinyint(4) | 
| id | bigint(20) unsigned | 
| created_at | timestamp | 
| updated_at | timestamp | 


### group_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### groups
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### groups_accounts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| groups_id | int(10) unsigned | 
| accounts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### input_masks
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| created_at | timestamp | 
| updated_at | timestamp | 


### input_types
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(128) | 
| mask | varchar(128) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### invoice_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### invoices
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| status | int(11) | 
| currency | int(11) | 
| amount | double | 
| tax | double | 
| total | double | 
| subtotal | double | 
| discount | double | 
| billing_address | varchar(255) | 
| billing_city | varchar(255) | 
| billing_zip | varchar(255) | 
| billing_state | int(11) | 
| billing_country | int(11) | 
| shipping_address | varchar(255) | 
| shipping_city | varchar(255) | 
| shipping_zip | varchar(255) | 
| shipping_state | int(11) | 
| shipping_country | int(11) | 
| sign_date | int(11) | 
| expire_date | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### lead_sources
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### lead_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### lead_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### leads
| Field name | Type |
| --- | --- |
| first_name | varchar(255) | 
| last_name | varchar(255) | 
| email | varchar(255) | 
| phone | varchar(255) | 
| fax | varchar(255) | 
| website | varchar(255) | 
| address | varchar(255) | 
| city | varchar(255) | 
| state | int(11) | 
| zip | varchar(255) | 
| country | int(11) | 
| description | varchar(255) | 
| status | int(11) | 
| email_receive | tinyint(1) | 
| assigned_to | int(11) | 
| lead_type | int(11) | 
| lead_source | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### leads_accounts_opportunities
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| leads_id | int(10) unsigned | 
| accounts_id | int(10) unsigned | 
| opportunities_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### lineitems
| Field name | Type |
| --- | --- |
| product_id | int(11) | 
| quantity | int(11) | 
| price | double | 
| unit_price | double | 
| cost | double | 
| discount | double | 
| discount_type | int(11) | 
| taxes | double | 
| gross | double | 
| net | double | 
| description | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### logs
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| module_id | int(11) | 
| type | varchar(16) | 
| message | varchar(200) | 
| user_id | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### meeting_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### meeting_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### meetings
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| start_date | int(11) | 
| end_date | int(11) | 
| start_time | int(11) | 
| end_time | int(11) | 
| reminder_time | int(11) | 
| location | varchar(255) | 
| phone | varchar(255) | 
| link | varchar(255) | 
| meeting_password | varchar(255) | 
| types | int(11) | 
| status | int(11) | 
| assigned_to | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### migrations
| Field name | Type |
| --- | --- |
| id | int(10) unsigned | 
| migration | varchar(255) | 
| batch | int(11) | 


### module_convertables
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| primary_module_id | int(11) | 
| module_id | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### module_groups
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(255) | 
| label | varchar(255) | 
| view_order | int(11) | 


### module_subpanels
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| subpanel_filter | varchar(255) | 
| name | varchar(255) | 
| label | varchar(255) | 
| module_id | varchar(255) | 
| list_size | int(11) | 
| list_order_column | varchar(255) | 
| list_order | varchar(255) | 
| relationship_id | int(11) | 
| status | int(11) | 
| saved_search_id | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### modules
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(100) | 
| label | varchar(255) | 
| description | varchar(255) | 
| status | int(11) | 
| faker_seed | int(11) | 
| create_table | int(11) | 
| view_order | int(11) | 
| admin | int(11) | 
| parent_id | int(11) | 
| primary | int(11) | 
| icon | varchar(128) | 
| module_group_id | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### modules_datalets
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| modules_id | int(10) unsigned | 
| datalets_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### modules_fields
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| modules_id | int(10) unsigned | 
| fields_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### modules_subpanels
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| modules_id | int(10) unsigned | 
| module_subpanels_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes
| Field name | Type |
| --- | --- |
| subject | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| file_location | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes_accounts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| notes_id | int(10) unsigned | 
| accounts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes_cases
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| documents_id | int(10) unsigned | 
| cases_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes_contracts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| notes_id | int(10) unsigned | 
| contracts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes_meetings
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| notes_id | int(10) unsigned | 
| meetings_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes_opportunities
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| notes_id | int(10) unsigned | 
| opportunities_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes_tasks
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| notes_id | int(10) unsigned | 
| tasks_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### notes_users
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| notes_id | int(10) unsigned | 
| users_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunities
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| assigned_to | int(11) | 
| type | int(11) | 
| amount | double | 
| probability | int(11) | 
| close_date | int(11) | 
| status | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunities_cases
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| opportunities_id | int(10) unsigned | 
| cases_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunities_contacts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| accounts_id | int(10) unsigned | 
| opportunities_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunities_contracts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| opportunities_id | int(10) unsigned | 
| contracts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunities_meetings
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| opportunities_id | int(10) unsigned | 
| meetings_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunities_quotes
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| opportunities_id | int(10) unsigned | 
| quotes_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunities_quotes_accounts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| opportunities_id | int(10) unsigned | 
| quotes_id | int(10) unsigned | 
| accounts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunity_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### opportunity_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### orders
| Field name | Type |
| --- | --- |
| first_name | varchar(255) | 
| last_name | varchar(255) | 
| email | varchar(255) | 
| phone | varchar(255) | 
| status | int(11) | 
| currency | int(11) | 
| amount | double | 
| tax | double | 
| total | double | 
| subtotal | double | 
| discount | double | 
| billing_address | varchar(255) | 
| billing_city | varchar(255) | 
| billing_zip | varchar(255) | 
| billing_state | int(11) | 
| billing_country | int(11) | 
| shipping_address | varchar(255) | 
| shipping_city | varchar(255) | 
| shipping_zip | varchar(255) | 
| shipping_state | int(11) | 
| shipping_country | int(11) | 
| product | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### password_resets
| Field name | Type |
| --- | --- |
| email | varchar(255) | 
| token | varchar(255) | 
| created_at | timestamp | 


### permissions
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| module_id | int(11) | 
| role_id | int(11) | 
| can_read | int(11) | 
| can_write | int(11) | 
| can_delete | int(11) | 
| can_export | int(11) | 
| can_import | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### personal_access_tokens
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| tokenable_type | varchar(255) | 
| tokenable_id | bigint(20) unsigned | 
| name | varchar(255) | 
| token | varchar(64) | 
| abilities | text | 
| last_used_at | timestamp | 
| created_at | timestamp | 
| updated_at | timestamp | 


### products
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### project_priorities
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### project_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### project_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### projects
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| status | int(11) | 
| priority | int(11) | 
| type | int(11) | 
| start_date | int(11) | 
| end_date | int(11) | 
| due_date | int(11) | 
| completed_date | int(11) | 
| estimated_hours | int(11) | 
| actual_hours | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### projects_accounts
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| projects_id | int(10) unsigned | 
| accounts_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### projects_tasks
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| projects_id | int(10) unsigned | 
| tasks_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### quote_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### quotes
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| status | int(11) | 
| currency | int(11) | 
| amount | double | 
| tax | double | 
| total | double | 
| subtotal | double | 
| discount | double | 
| billing_address | varchar(255) | 
| billing_city | varchar(255) | 
| billing_zip | varchar(255) | 
| billing_state | int(11) | 
| billing_country | int(11) | 
| shipping_address | varchar(255) | 
| shipping_city | varchar(255) | 
| shipping_zip | varchar(255) | 
| shipping_state | int(11) | 
| shipping_country | int(11) | 
| expire_date | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### relationship_modules
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| module_id | int(11) | 
| relationship_id | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### relationships
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(255) | 
| modules | varchar(255) | 
| related_field_types | varchar(255) | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### roles
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### settings
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(255) | 
| value | varchar(255) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### states
| Field name | Type |
| --- | --- |
| code | varchar(255) | 
| abbreviation | varchar(255) | 
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### subpanel_fields
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| field_id | int(11) | 
| subpanel_id | int(11) | 
| label | varchar(255) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### task_priorities
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### task_status
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### task_types
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### tasks
| Field name | Type |
| --- | --- |
| subject | varchar(255) | 
| description | varchar(255) | 
| assigned_to | int(11) | 
| task_types | int(11) | 
| status | int(11) | 
| task_priority | int(11) | 
| due_date | int(11) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### themes
| Field name | Type |
| --- | --- |
| name | varchar(255) | 
| id | bigint(20) unsigned | 
| slug | varchar(64) | 
| soft_delete | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### user_meetings
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| users_id | int(10) unsigned | 
| meetings_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### users
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(255) | 
| email | varchar(255) | 
| email_verified_at | timestamp | 
| password | varchar(255) | 
| role_id | int(11) | 
| slug | varchar(255) | 
| remember_token | varchar(100) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### users_tasks
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| users_id | int(10) unsigned | 
| tasks_id | int(10) unsigned | 
| status | int(11) | 
| created_at | timestamp | 
| updated_at | timestamp | 


### workflow_actions
| Field name | Type |
| --- | --- |
| id | bigint(20) unsigned | 
| name | varchar(255) | 
| created_at | timestamp | 
| updated_at | timestamp | 


