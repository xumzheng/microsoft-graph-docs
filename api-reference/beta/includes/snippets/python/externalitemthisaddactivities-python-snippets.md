---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Add_activities_post_request_body()
activities_external_activity1 = External_activity()
activities_external_activity1.@odata_type = '#microsoft.graph.externalConnectors.externalActivity'

activities_external_activity1.type(ExternalActivityType.String('externalactivitytype.string'))

activities_external_activity1.startDateTime = DateTime('String (timestamp)')


activitiesArray []= activitiesExternalActivity1;
request_body.activities(activitiesArray)





result = await client.connections.by_connection_id('externalConnection-id').items.by_item_id('externalItem-id').microsoft_graph_external_connector_add_activities.post(request_body = request_body)


```