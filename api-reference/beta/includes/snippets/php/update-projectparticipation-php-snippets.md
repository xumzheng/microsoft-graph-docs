---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ProjectParticipation();


$requestRequestBody->setAllowedAudiences(new AllowedAudiences('organization'));

$client = new CompanyDetail();
$requestRequestBody->setClient($client);


$client->setDepartment('Corporate Marketing');
$client->setWebUrl('https://www.contoso.com');

$result =  $graphClient->me()->profile()->projectsById('projectParticipation-id')->patch($requestRequestBody);


```