---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConnectorGroup()
request_body.setName('name-value')

request_body.setRegion(ConnectorGroupRegion('region-value'))



result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').connectorGroups_by_id('connectorGroup-id').patch(request_body, headers=)


```