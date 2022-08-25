# Task

## Operations

### Create

POST request accepts either a Task object or a list of thereof.

When you try setting metafield that's not editable, the API will return HTTP error 400

### List

It's possible to search by metafields using query parameters. The syntax is:
metafields__{namespace}:{key}__{operator}

Known operators are
- no operator - full string search (skip the __ in the end)
- contains - substring search
- in - enum search

## Fields

### category

type: string enum

- assignment
- pick-up
- drop-off

Pick-ups and drop-offs are used in the [Route optimisation](route_optimisations.md), but it's not required that both pick-up and drop-off tasks are created for any given Order.

### external_id

Type: string (max 100 characters)

It's used just to overwrite data. If you wish to have a duplicate with a same number use either “reference” or a new “metafield”.
External ID is used by customers who wish to overwrite information in a task after it has been completed or cancelled.

### reference

Type: string (max 100 characters)

The field has unclear special meaning. The user interface will highlight all tasks with matching reference when any of then is selected in the dashboard.

### metafields

"[Metafields](metafields.md)" are just custom fields, defined in the account. API and UI for editing is available.

### size

Not in use
