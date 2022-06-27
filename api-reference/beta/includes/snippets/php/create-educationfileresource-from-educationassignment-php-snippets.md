---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationAssignmentResource();


$requestRequestBody->setDistributeForStudentWork(False);

$resource = new EducationResource();
$requestRequestBody->setResource($resource);


$resource->setDisplayName('article.pdf');
$resourceAdditionalData = [
	"@odata.type" => '#microsoft.graph.educationFileResource',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->resources()->post($requestRequestBody);


```