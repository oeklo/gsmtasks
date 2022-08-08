# Task

## Operations

### Create

POST request accepts either a Task object or a list of thereof.

## Fields

### category

- assignment
- pick-up
- drop-off
- warehouse - not in use

### external_id

Type: string (max 100 characters)

It's used just to overwrite data. If you wish to have a duplicate with a same number use either “reference” or a new “metafield”.
External ID is used by customers who wish to overwrite information in a task after it has been completed or cancelled.

### metafields

"Metafields" are just custom fields, defined in the account. API and UI for editing is available.

When you try setting metafield that's not editable, the API will return HTTP error 400

### size

Not in use
