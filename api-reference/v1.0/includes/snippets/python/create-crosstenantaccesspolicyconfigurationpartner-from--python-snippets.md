---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicyConfigurationPartner()
request_body.tenantId = '3d0f5dec-5d3d-455c-8016-e2af1ae4d31a'

b2b_direct_connect_outbound = CrossTenantAccessPolicyB2BSetting()
b2b_direct_connect_outbound_users_and_groups = CrossTenantAccessPolicyTargetConfiguration()
b2bDirectConnectOutboundUsersAndGroups.AccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'))

targets_cross_tenant_access_policy_target1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.target = '6f546279-4da5-4b53-a095-09ea0cef9971'

targetsCrossTenantAccessPolicyTarget1.TargetType(CrossTenantAccessPolicyTargetType('group'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bDirectConnectOutboundUsersAndGroups.targets(targetsArray)



b2bDirectConnectOutbound.users_and_groups = b2bDirectConnectOutboundUsersAndGroups

request_body.b2b_direct_connect_outbound = b2bDirectConnectOutbound
b2b_direct_connect_inbound = CrossTenantAccessPolicyB2BSetting()
b2b_direct_connect_inbound_applications = CrossTenantAccessPolicyTargetConfiguration()
b2bDirectConnectInboundApplications.AccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('allowed'))

targets_cross_tenant_access_policy_target1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.target = 'Office365'

targetsCrossTenantAccessPolicyTarget1.TargetType(CrossTenantAccessPolicyTargetType('application'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bDirectConnectInboundApplications.targets(targetsArray)



b2bDirectConnectInbound.applications = b2bDirectConnectInboundApplications

request_body.b2b_direct_connect_inbound = b2bDirectConnectInbound



result = await client.policies.crossTenantAccessPolicy.partners.post(request_body = request_body)


```