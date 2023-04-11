---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcUserSetting()
request_body.@odatatype = '#microsoft.graph.cloudPcUserSetting'

request_body.displayName = 'Example'

request_body.selfServiceEnabled = true

restorePointSetting = CloudPcRestorePointSetting()
restorePointSetting.frequencyInHours = 16

restorePointSetting.userRestoreEnabled = true


request_body.restorePointSetting = restorePointSetting
request_body.localAdminEnabled = false



request_configuration = CloudPcUserSettingRequestBuilderPatchRequestConfiguration(
)


result = await client.deviceManagement.virtualEndpoint.userSettings_by_id('cloudPcUserSetting-id').patch(request_body = request_body)


```