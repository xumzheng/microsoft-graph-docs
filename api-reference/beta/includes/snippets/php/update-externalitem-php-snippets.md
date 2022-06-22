---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExternalItem();


$aclArray = [];

$acl1 = new Acl();

$acl1->setType(new AclType('everyone'));
$acl1->setValue('67a141d8-cf4e-4528-ba07-bed21bfacd2d');
$acl1->setAccessType(new AccessType('grant'));

$aclArray []= $acl1;
$requestRequestBody->setAcl($aclArray);
$result =  $graphClient->external()->connectionsById('externalConnection-id')->itemsById('externalItem-id')->patch($requestRequestBody);


```