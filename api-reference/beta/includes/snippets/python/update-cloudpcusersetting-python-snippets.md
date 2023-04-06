---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcUserSetting()
request_body.set@odatatype('#microsoft.graph.cloudPcUserSetting')

request_body.setDisplayName('Example')

request_body.setSelfServiceEnabled(true)

restorePointSetting = CloudPcRestorePointSetting()
restorePointSetting.setFrequencyInHours(16)

restorePointSetting.setUserRestoreEnabled(true)


request_body.setRestorePointSetting($restorePointSetting)
request_body.setLocalAdminEnabled(false)


request_config = CloudPcUserSettingRequestBuilderPatchRequestConfiguration(
request_config = CloudPcUserSettingRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.deviceManagement.virtualEndpoint.userSettings_by_id('cloudPcUserSetting-id').patch(request_body, headers=)


```