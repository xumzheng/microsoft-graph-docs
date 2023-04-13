---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AssignPostRequestBody()
assignments_cloud_pc_provisioning_policy_assignment1 = CloudPcProvisioningPolicyAssignment()
assignmentsCloudPcProvisioningPolicyAssignment1.id = 'b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff'

assignments_cloud_pc_provisioning_policy_assignment1_target = CloudPcManagementAssignmentTarget()
assignmentsCloudPcProvisioningPolicyAssignment1Target.@odatatype = 'microsoft.graph.cloudPcManagementGroupAssignmentTarget'

additionalData = [
'groupId' => '64ff06de-9c00-4a5a-98b5-7f5abe26ffff', 
];
assignmentsCloudPcProvisioningPolicyAssignment1Target.additionaldata(additionalData)



assignmentsCloudPcProvisioningPolicyAssignment1.target = assignmentsCloudPcProvisioningPolicyAssignment1Target

assignmentsArray []= assignmentsCloudPcProvisioningPolicyAssignment1;
request_body.assignments(assignmentsArray)


additionalData = [
'@odata.type' => '#microsoft.graph.cloudPcProvisioningPolicyAssignment', 
];
request_body.additionaldata(additionalData)





await client.deviceManagement.virtualEndpoint.provisioningPolicies_by_id('cloudPcProvisioningPolicy-id').assign.post(request_body = request_body)


```