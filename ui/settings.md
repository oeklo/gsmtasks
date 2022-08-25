# [Settings](https://app.gsmtasks.com/settings/)

## [Custom fields](https://app.gsmtasks.com/settings/metafields) (A.K.A Metafields)

### Caveats

- When creating a new metafield you must select at least on of the "Show in", otherwise the field doesn't show in the
  settings view or in the API. The field exists, but it's inaccessible and a new field with the same namespace & key pair can't be created. 
  In other words it's not possible to have a custom field that's visible only to the API.
