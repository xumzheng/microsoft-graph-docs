---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ScopedRoleMembership();
$requestBody.setRoleId('roleId-value');

$roleMemberInfo = new Identity();
$roleMemberInfo.setId('id-value');


$requestBody.setRoleMemberInfo($roleMemberInfo);


$requestResult = $graphServiceClient.administrativeUnitsById('administrativeUnit-id').scopedRoleMembers().post($requestBody);


```