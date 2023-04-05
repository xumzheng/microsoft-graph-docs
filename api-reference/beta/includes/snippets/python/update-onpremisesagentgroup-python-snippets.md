---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnPremisesAgentGroup()
request_body.setDisplayName('Group New Name')



result = await client.onPremisesPublishingProfilesby_id('onPremisesPublishingProfile-id')_agentGroupsby_id('onPremisesAgentGroup-id').patch(request_body)


```