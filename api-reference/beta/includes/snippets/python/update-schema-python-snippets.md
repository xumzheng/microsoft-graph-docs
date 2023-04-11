---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Schema()
request_body.baseType = 'microsoft.graph.externalItem'

propertiesProperty1 = Property()
propertiesProperty1.name = 'ticketTitle'

propertiesProperty1.Type(PropertyType('string'))

propertiesProperty1.isSearchable = true

propertiesProperty1.isRetrievable = true

propertiesProperty1.Labels([propertiesProperty1.Label(Label('title'))
])


propertiesArray []= propertiesProperty1;
propertiesProperty2 = Property()
propertiesProperty2.name = 'priority'

propertiesProperty2.Type(PropertyType('string'))

propertiesProperty2.isQueryable = true

propertiesProperty2.isRetrievable = true

propertiesProperty2.isSearchable = false


propertiesArray []= propertiesProperty2;
propertiesProperty3 = Property()
propertiesProperty3.name = 'assignee'

propertiesProperty3.Type(PropertyType('string'))

propertiesProperty3.isRetrievable = true


propertiesArray []= propertiesProperty3;
request_body.properties(propertiesArray)





result = await client.external.connections_by_id('externalConnection-id').schema.patch(request_body = request_body)


```