---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonAnnotation();


$requestRequestBody->setAllowedAudiences(new AllowedAudiences('organization'));
$result =  $graphClient->usersById('user-id')->profile()->notesById('personAnnotation-id')->patch($requestRequestBody);


```