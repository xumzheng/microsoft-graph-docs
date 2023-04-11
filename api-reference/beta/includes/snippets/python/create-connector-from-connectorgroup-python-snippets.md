---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.@odataid = 'https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}'



request_configuration = RefRequestBuilderPostRequestConfiguration(
)


await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').connectorGroups_by_id('connectorGroup-id').members.ref.post(request_body = request_body)


```