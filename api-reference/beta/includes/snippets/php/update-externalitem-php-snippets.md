---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExternalItem();


$aclArray = [];

$aclacl1 = new Acl();

$aclacl1->setType(new AclType('everyone'));
$aclacl1->setValue('67a141d8-cf4e-4528-ba07-bed21bfacd2d');
$aclacl1->setAccessType(new AccessType('grant'));

$aclArray []= $aclacl1;
$requestRequestBody->setAcl($aclArray);
$result =  $graphClient->external()->connectionsById('externalConnection-id')->itemsById('externalItem-id')->patch($requestRequestBody);


```