---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AssignPostRequestBody()
assignmentsCloudPcProvisioningPolicyAssignment1 = CloudPcProvisioningPolicyAssignment()
assignmentsCloudPcProvisioningPolicyAssignment1.setId('b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff')

assignmentsCloudPcProvisioningPolicyAssignment1Target = CloudPcManagementAssignmentTarget()
assignmentsCloudPcProvisioningPolicyAssignment1Target.set@odatatype('microsoft.graph.cloudPcManagementGroupAssignmentTarget')

additionalData = [
'groupId' => '64ff06de-9c00-4a5a-98b5-7f5abe26ffff', 
];
assignmentsCloudPcProvisioningPolicyAssignment1Target.setAdditionalData(additionalData)



assignmentsCloudPcProvisioningPolicyAssignment1.setTarget($assignmentsCloudPcProvisioningPolicyAssignment1Target)

assignmentsArray []= assignmentsCloudPcProvisioningPolicyAssignment1;
request_body.setAssignments(assignmentsArray)


additionalData = [
'@odata.type' => '#microsoft.graph.cloudPcProvisioningPolicyAssignment', 
];
request_body.setAdditionalData(additionalData)




await client.deviceManagement.virtualEndpoint.provisioningPoliciesById('cloudPcProvisioningPolicy-id').assign.post(request_body)


```