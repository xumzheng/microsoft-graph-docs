---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationSchool();


$requestRequestBody->setDisplayName('Fabrikam Arts High School');
$requestRequestBody->setDescription('Magnate school for the arts. Los Angeles School District');
$result =  $graphClient->education()->schoolsById('educationSchool-id')->patch($requestRequestBody);


```