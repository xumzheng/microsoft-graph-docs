---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationSubmissionResource();



$resource = new EducationResource();
$requestRequestBody->setResource($resource);


$resource->setDisplayName('Report.docx');
$resourceAdditionalData = [
	"@odata.type" => 'microsoft.graph.educationWordResource',
	"fileUrl" => 'https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->resources()->post($requestRequestBody);


```