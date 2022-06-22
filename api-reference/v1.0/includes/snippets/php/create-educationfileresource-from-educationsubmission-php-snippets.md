---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationSubmissionResource();



$resource = new EducationResource();
$requestRequestBody->setResource($resource);


$resource->setDisplayName('_FTP_EDC-61424749-250820211136.pdf');
$resourceAdditionalData = [
	"fileUrl" => 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3',
	"@odata.type" => '#microsoft.graph.educationFileResource',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->resources()->post($requestRequestBody);


```