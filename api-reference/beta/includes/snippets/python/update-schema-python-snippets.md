---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Schema()
request_body.baseType = 'microsoft.graph.externalItem'

properties_property1 = Property()
propertiesProperty1.name = 'ticketTitle'

propertiesProperty1.Type(PropertyType('string'))

propertiesProperty1.is_searchable = True

propertiesProperty1.is_retrievable = True

propertiesProperty1.Labels([propertiesProperty1.Label(Label('title'))
])


propertiesArray []= propertiesProperty1;
properties_property2 = Property()
propertiesProperty2.name = 'priority'

propertiesProperty2.Type(PropertyType('string'))

propertiesProperty2.is_queryable = True

propertiesProperty2.is_retrievable = True

propertiesProperty2.is_searchable = False


propertiesArray []= propertiesProperty2;
properties_property3 = Property()
propertiesProperty3.name = 'assignee'

propertiesProperty3.Type(PropertyType('string'))

propertiesProperty3.is_retrievable = True


propertiesArray []= propertiesProperty3;
request_body.properties(propertiesArray)





result = await client.external.connections_by_id('externalConnection-id').schema.patch(request_body = request_body)


```