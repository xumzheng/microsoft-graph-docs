---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ScopedRoleMembership();
requestBody.setRoleId('roleId-value');

roleMemberInfo = Identity();
roleMemberInfo.setId('id-value');


requestBody.setRoleMemberInfo($roleMemberInfo);


result = awaitclient.administrativeUnitsById('administrativeUnit-id').scopedRoleMembers().post(requestBody);


```