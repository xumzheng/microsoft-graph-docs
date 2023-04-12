---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AssignPostRequestBody()
assignmentsCloudPcUserSettingAssignment1 = CloudPcUserSettingAssignment()
assignmentsCloudPcUserSettingAssignment1.id = 'b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff'

assignmentsCloudPcUserSettingAssignment1Target = CloudPcManagementAssignmentTarget()
assignmentsCloudPcUserSettingAssignment1Target.@odatatype = 'microsoft.graph.cloudPcManagementGroupAssignmentTarget'

additionalData = [
'groupId' => '64ff06de-9c00-4a5a-98b5-7f5abe26ffff', 
];
assignmentsCloudPcUserSettingAssignment1Target.additionaldata(additionalData)



assignmentsCloudPcUserSettingAssignment1.target = assignmentsCloudPcUserSettingAssignment1Target

assignmentsArray []= assignmentsCloudPcUserSettingAssignment1;
request_body.assignments(assignmentsArray)





await client.deviceManagement.virtualEndpoint.userSettings_by_id('cloudPcUserSetting-id').assign.post(request_body = request_body)


```