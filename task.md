# Task

## Fields

### size

Type: signed int 32bit

This is an arbitrary number describind the size of the task.

When planning a route, total of all tasks sizes must not exceede account_role.vehicle_capacity_field

Works only for tasks of category pick-up or drop-off (untested, might require an order with a pick-up and a drop-off tasks).

### category

- assignment
- pick-up
- drop-off
- warehouse - undocumented

### external_id

Type: string (max 100 characters)

Unique for client (most likely).

When creating a new task (POST) the external_id is checked and if another task exists with the same external_id, no task is created and the old task is returned.

### metafields

When you try setting metafield that's not editable, the API will return HTTP error 400
