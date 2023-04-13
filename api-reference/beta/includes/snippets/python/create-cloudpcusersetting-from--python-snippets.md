---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcUserSetting()
request_body.@odatatype = '#microsoft.graph.cloudPcUserSetting'

request_body.displayName = 'Example'

request_body.self_service_enabled = False

request_body.local_admin_enabled = True

restore_point_setting = CloudPcRestorePointSetting()
restorePointSetting.frequency_in_hours = 16

restorePointSetting.user_restore_enabled = True


request_body.restore_point_setting = restorePointSetting



result = await client.deviceManagement.virtualEndpoint.userSettings.post(request_body = request_body)


```