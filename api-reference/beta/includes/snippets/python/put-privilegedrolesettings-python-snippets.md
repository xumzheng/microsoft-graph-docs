---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SettingsPutRequestBody()
additional_data = [
'id' => '9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3', 
'elevation_duration' => 'PT8H', 
'notification_to_user_on_elevation' => false,
'ticketing_info_on_elevation' => true,
'mfa_on_elevation' => false,
'max_elavation_duration' => 'PT0S', 
'min_elevation_duration' => 'PT0S', 
'last_global_admin' => false,
'is_mfa_on_elevation_configurable' => true,
'approval_on_elevation' => false,
'approver_ids' => ['e2b2a2fb-13d7-495c-adc9-941fe966793f', '22770e3f-b9b4-418e-9dea-d0e3d2f275dd', ],
];
request_body.additional_data(additional_data)





await client.privileged_roles.by_privileged_role_id('privilegedRole-id').settings.put(request_body = request_body)


```