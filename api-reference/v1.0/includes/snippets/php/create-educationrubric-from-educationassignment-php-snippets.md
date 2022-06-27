---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReferenceUpdateSchema();


$requestRequestBody->set@odata.id('https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d');
$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->rubric()->ref()->put($requestRequestBody);


```