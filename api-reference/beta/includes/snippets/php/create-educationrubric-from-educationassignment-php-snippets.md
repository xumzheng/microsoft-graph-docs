---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReferenceUpdateSchema();


$requestRequestBody->set@odata.id('https://graph.microsoft.com/v1.0/education/me/rubrics/{id}');
$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->rubric()->ref()->put($requestRequestBody);


```