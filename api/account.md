# Account

## Fields

### dashboard_task_template

type: string (no known size limit)

Default value:
```jsp
<%= contact.name %>\r\n<%= address.raw_address %>
```

A template for a single entry in the task list on the web application.

Template can have three rows, where the first displayed in a big font,
second and third are displayed in a small font.

The second row also displays [task.category](task.mdategory) to the left, and time part of complete_after and complete before fields. That's not configurable.

Fields in the same row are separated with ' / ' but I'm not sure if it's hardcoded or not.

There is also separate template for mobile app, but it's not available via the API.

Templates can be only modified by contacting the GSMTasks support.

It's done quite quickly, but in my case they've tried to be smarter and did a bit different change than I've asked. So if you're removing the default fields, mention that you really want it removed.
