---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicyConfigurationDefault()
b2bCollaborationOutbound = CrossTenantAccessPolicyB2BSetting()
b2bCollaborationOutboundUsersAndGroups = CrossTenantAccessPolicyTargetConfiguration()
b2bCollaborationOutboundUsersAndGroups.setAccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'))

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.setTarget('0be493dc-cb56-4a53-936f-9cf64410b8b0')

targetsCrossTenantAccessPolicyTarget1.setTargetType(CrossTenantAccessPolicyTargetType('group'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bCollaborationOutboundUsersAndGroups.setTargets(targetsArray)



b2bCollaborationOutbound.setUsersAndGroups($b2bCollaborationOutboundUsersAndGroups)
b2bCollaborationOutboundApplications = CrossTenantAccessPolicyTargetConfiguration()
b2bCollaborationOutboundApplications.setAccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'))

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.setTarget('AllApplications')

targetsCrossTenantAccessPolicyTarget1.setTargetType(CrossTenantAccessPolicyTargetType('application'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bCollaborationOutboundApplications.setTargets(targetsArray)



b2bCollaborationOutbound.setApplications($b2bCollaborationOutboundApplications)

request_body.setB2bCollaborationOutbound($b2bCollaborationOutbound)


result = await client.policies_crossTenantAccessPolicy_default.patch(request_body)


```