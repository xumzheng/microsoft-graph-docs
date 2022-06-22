---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationSubmissionResource();



$resource = new EducationResource();
$requestRequestBody->setResource($resource);


$resource->setDisplayName('Wikipedia');
$resourceAdditionalData = [
	"link" => 'https://en.wikipedia.org/wiki/Main_Page',
	"@odata.type" => '#microsoft.graph.educationLinkResource',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->resources()->post($requestRequestBody);


```