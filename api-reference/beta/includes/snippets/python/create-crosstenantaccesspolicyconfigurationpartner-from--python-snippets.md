---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CrossTenantAccessPolicyConfigurationPartner();
request_body.setTenantId('3d0f5dec-5d3d-455c-8016-e2af1ae4d31a');

b2bDirectConnectOutbound = CrossTenantAccessPolicyB2BSetting();
b2bDirectConnectOutboundUsersAndGroups = CrossTenantAccessPolicyTargetConfiguration();
b2bDirectConnectOutboundUsersAndGroups.setAccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'));

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget();
targetsCrossTenantAccessPolicyTarget1.setTarget('6f546279-4da5-4b53-a095-09ea0cef9971');

targetsCrossTenantAccessPolicyTarget1.setTargetType(CrossTenantAccessPolicyTargetType('group'));


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bDirectConnectOutboundUsersAndGroups.setTargets(targetsArray);



b2bDirectConnectOutbound.setUsersAndGroups($b2bDirectConnectOutboundUsersAndGroups);

request_body.setB2bDirectConnectOutbound($b2bDirectConnectOutbound);
b2bDirectConnectInbound = CrossTenantAccessPolicyB2BSetting();
b2bDirectConnectInboundApplications = CrossTenantAccessPolicyTargetConfiguration();
b2bDirectConnectInboundApplications.setAccessType(CrossTenantAccessPolicyTargetConfigurationAccessType('allowed'));

targetsCrossTenantAccessPolicyTarget1 = CrossTenantAccessPolicyTarget();
targetsCrossTenantAccessPolicyTarget1.setTarget('Office365');

targetsCrossTenantAccessPolicyTarget1.setTargetType(CrossTenantAccessPolicyTargetType('application'));


targetsArray []= targetsCrossTenantAccessPolicyTarget1;
b2bDirectConnectInboundApplications.setTargets(targetsArray);



b2bDirectConnectInbound.setApplications($b2bDirectConnectInboundApplications);

request_body.setB2bDirectConnectInbound($b2bDirectConnectInbound);


result = await client.policies.crossTenantAccessPolicy.partners.post(request_body);


```