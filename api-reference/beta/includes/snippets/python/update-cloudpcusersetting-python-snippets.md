---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcUserSetting()
request_body.@odatatype = '#microsoft.graph.cloudPcUserSetting'

request_body.displayName = 'Example'

request_body.self_service_enabled = True

restore_point_setting = CloudPcRestorePointSetting()
restorePointSetting.frequency_in_hours = 16

restorePointSetting.user_restore_enabled = True


request_body.restore_point_setting = restorePointSetting
request_body.local_admin_enabled = False




result = await client.deviceManagement.virtualEndpoint.userSettings_by_id('cloudPcUserSetting-id').patch(request_body = request_body)


```