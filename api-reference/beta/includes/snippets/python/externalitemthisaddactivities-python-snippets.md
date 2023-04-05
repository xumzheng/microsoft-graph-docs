---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddActivitiesPostRequestBody()
activitiesExternalActivity1 = ExternalActivity()
activitiesExternalActivity1.set@odatatype('#microsoft.graph.externalConnectors.externalActivity')

activitiesExternalActivity1.setType(ExternalActivityType('string'))

activitiesExternalActivity1.setStartDateTime(DateTime('String (timestamp)'))


activitiesArray []= activitiesExternalActivity1;
request_body.setActivities(activitiesArray)




result = await client.connectionsby_id('externalConnection-id')_itemsby_id('externalItem-id')_externalConnectorsaddActivities.post(request_body)


```