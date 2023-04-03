---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ScopedRoleMembership();
requestBody.setRoleId('roleId-value');

roleMemberInfo = Identity();
roleMemberInfo.setId('id-value');


requestBody.setRoleMemberInfo($roleMemberInfo);


requestResult = graphServiceClient.directory().administrativeUnitsById('administrativeUnit-id').scopedRoleMembers().post(requestBody);


```