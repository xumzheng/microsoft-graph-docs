---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.@odataid = 'https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6'



request_configuration = RefRequestBuilderPostRequestConfiguration(
)


await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').connectors_by_id('connector-id').memberOf.ref.post(request_body = request_body)


```