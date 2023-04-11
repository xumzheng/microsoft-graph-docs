---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicyConfigurationDefault()
b2bCollaborationOutbound = CrossTenantAccessPolicyB2BSetting()
b2bCollaborationOutboundUsersAndGroups = CrossTenantAccessPolicyTargetConfiguration()
b2bCollaborationOutboundUsersAndGroups.AccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'))

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.target = '0be493dc-cb56-4a53-936f-9cf64410b8b0'

targetsCrossTenantAccessPolicyTarget1.TargetType(CrossTenantAccessPolicyTargetType('group'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bCollaborationOutboundUsersAndGroups.targets(targetsArray)



b2bCollaborationOutbound.usersAndGroups = b2bCollaborationOutboundUsersAndGroups
b2bCollaborationOutboundApplications = CrossTenantAccessPolicyTargetConfiguration()
b2bCollaborationOutboundApplications.AccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'))

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.target = 'AllApplications'

targetsCrossTenantAccessPolicyTarget1.TargetType(CrossTenantAccessPolicyTargetType('application'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bCollaborationOutboundApplications.targets(targetsArray)



b2bCollaborationOutbound.applications = b2bCollaborationOutboundApplications

request_body.b2bCollaborationOutbound = b2bCollaborationOutbound



result = await client.policies.crossTenantAccessPolicy.default.patch(request_body = request_body)


```