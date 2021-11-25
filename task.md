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
