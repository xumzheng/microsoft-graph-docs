---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAudienceByIdPostRequestBody()
request_body.memberEntityType = 'String'

request_body.AddMembers(['String', ])

request_body.RemoveMembers(['String', ])

request_body.AddExclusions(['String', ])

request_body.RemoveExclusions(['String', ])



request_configuration = UpdateAudienceByIdRequestBuilderPostRequestConfiguration(
)


await client.admin.windows.updates.deployments_by_id('deployment-id').audience.windowsUpdatesupdateAudienceById.post(request_body = request_body)


```