---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossTenantAccessPolicyConfigurationPartner()
request_body.tenantId = '3d0f5dec-5d3d-455c-8016-e2af1ae4d31a'

b2bDirectConnectOutbound = CrossTenantAccessPolicyB2BSetting()
b2bDirectConnectOutboundUsersAndGroups = CrossTenantAccessPolicyTargetConfiguration()
b2bDirectConnectOutboundUsersAndGroups.AccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'))

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.target = '6f546279-4da5-4b53-a095-09ea0cef9971'

targetsCrossTenantAccessPolicyTarget1.TargetType(CrossTenantAccessPolicyTargetType('group'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bDirectConnectOutboundUsersAndGroups.targets(targetsArray)



b2bDirectConnectOutbound.usersAndGroups = b2bDirectConnectOutboundUsersAndGroups

request_body.b2bDirectConnectOutbound = b2bDirectConnectOutbound
b2bDirectConnectInbound = CrossTenantAccessPolicyB2BSetting()
b2bDirectConnectInboundApplications = CrossTenantAccessPolicyTargetConfiguration()
b2bDirectConnectInboundApplications.AccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('allowed'))

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget()
targetsCrossTenantAccessPolicyTarget1.target = 'Office365'

targetsCrossTenantAccessPolicyTarget1.TargetType(CrossTenantAccessPolicyTargetType('application'))


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bDirectConnectInboundApplications.targets(targetsArray)



b2bDirectConnectInbound.applications = b2bDirectConnectInboundApplications

request_body.b2bDirectConnectInbound = b2bDirectConnectInbound


request_configuration = PartnersRequestBuilderPostRequestConfiguration(
)


result = await client.policies.crossTenantAccessPolicy.partners.post(request_body = request_body)


```