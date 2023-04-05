---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConnectorGroup()
request_body.setName('name-value')

request_body.setIsDefault(false)



result = await client.onPremisesPublishingProfilesby_id('onPremisesPublishingProfile-id')_connectorGroups.post(request_body)


```