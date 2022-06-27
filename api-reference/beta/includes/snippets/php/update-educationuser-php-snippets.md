---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationUser();


$requestRequestBody->setDisplayName('Rogelio Cazares');
$requestRequestBody->setGivenName('Rogelio');
$requestRequestBody->setMiddleName('Fernando');
$requestRequestBody->setSurname('Cazares');
$result =  $graphClient->education()->usersById('educationUser-id')->patch($requestRequestBody);


```