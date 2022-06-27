---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationSubmissionResource();



$resource = new EducationResource();
$requestRequestBody->setResource($resource);


$resource->setDisplayName('state diagram.pptx');
$resourceAdditionalData = [
	"@odata.type" => '#microsoft.graph.educationPowerPointResource',
	"fileUrl" => 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RN3MHWWM7BNXJD2UD5OMRFEDKN2',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->resources()->post($requestRequestBody);


```