---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}')



await client.onPremisesPublishingProfilesby_id('onPremisesPublishingProfile-id')_connectorGroupsby_id('connectorGroup-id')_members_ref.post(request_body)


```