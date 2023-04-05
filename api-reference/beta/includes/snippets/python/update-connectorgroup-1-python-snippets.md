---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConnectorGroup()
request_body.setName('Connector Group Demo')



result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').connectorGroups.post(request_body)


```