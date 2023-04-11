---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcUserSetting()
request_body.@odatatype = '#microsoft.graph.cloudPcUserSetting'

request_body.displayName = 'Example'

request_body.selfServiceEnabled = false

request_body.localAdminEnabled = true

restorePointSetting = CloudPcRestorePointSetting()
restorePointSetting.frequencyInHours = 16

restorePointSetting.userRestoreEnabled = true


request_body.restorePointSetting = restorePointSetting


request_configuration = UserSettingsRequestBuilderPostRequestConfiguration(
)


result = await client.deviceManagement.virtualEndpoint.userSettings.post(request_body = request_body)


```