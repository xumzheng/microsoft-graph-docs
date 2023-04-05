---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAudienceByIdPostRequestBody()
request_body.setMemberEntityType('String')

request_body.setAddMembers(['String', ])

request_body.setRemoveMembers(['String', ])

request_body.setAddExclusions(['String', ])

request_body.setRemoveExclusions(['String', ])



await client.admin.windows.updates.deployments_by_id('deployment-id').audience.windowsUpdatesupdateAudienceById.post(request_body)


```