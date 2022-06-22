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


$resource->setDisplayName('homework example.PNG');
$resourceAdditionalData = [
	"@odata.type" => 'microsoft.graph.educationMediaResource',
	"fileUrl" => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->resources()->post($requestRequestBody);


```