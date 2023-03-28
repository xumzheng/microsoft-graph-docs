---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ExternalItem();
$aclAcl1 = new Acl();
$aclAcl1.setType(new AclType('everyone'));

$aclAcl1.setValue('67a141d8-cf4e-4528-ba07-bed21bfacd2d');

$aclAcl1.setAccessType(new AccessType('grant'));


$aclArray []= $aclAcl1;
$requestBody.setAcl($aclArray);




$requestResult = $graphServiceClient.external().connectionsById('externalConnection-id').itemsById('externalItem-id').patch($requestBody);


```