---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Schema()
request_body.setBaseType('microsoft.graph.externalItem')

propertiesProperty1 = Property()
propertiesProperty1.setName('ticketTitle')

propertiesProperty1.setType(PropertyType('string'))

propertiesProperty1.setIsSearchable(true)

propertiesProperty1.setIsRetrievable(true)

propertiesProperty1.setLabels([propertiesProperty1.setLabel(Label('title'))
])


propertiesArray []= propertiesProperty1;
propertiesProperty2 = Property()
propertiesProperty2.setName('priority')

propertiesProperty2.setType(PropertyType('string'))

propertiesProperty2.setIsQueryable(true)

propertiesProperty2.setIsRetrievable(true)

propertiesProperty2.setIsSearchable(false)


propertiesArray []= propertiesProperty2;
propertiesProperty3 = Property()
propertiesProperty3.setName('assignee')

propertiesProperty3.setType(PropertyType('string'))

propertiesProperty3.setIsRetrievable(true)


propertiesArray []= propertiesProperty3;
request_body.setProperties(propertiesArray)




result = await client.external.connections_by_id('externalConnection-id').schema.patch(request_body, headers=)


```