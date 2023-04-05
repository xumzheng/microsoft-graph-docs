---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcUserSetting()
request_body.set@odatatype('#microsoft.graph.cloudPcUserSetting')

request_body.setDisplayName('Example')

request_body.setSelfServiceEnabled(false)

request_body.setLocalAdminEnabled(true)

restorePointSetting = CloudPcRestorePointSetting()
restorePointSetting.setFrequencyInHours(16)

restorePointSetting.setUserRestoreEnabled(true)


request_body.setRestorePointSetting($restorePointSetting)


result = await client.deviceManagement.virtualEndpoint.userSettings.post(request_body)


```