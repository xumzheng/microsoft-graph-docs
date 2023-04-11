---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceUpdate()
request_body.@odataid = 'https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}'



request_configuration = RefRequestBuilderPutRequestConfiguration(
)


await client.applications_by_id('application-id').connectorGroup.ref.put(request_body = request_body)


```