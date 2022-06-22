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


$resource->setDisplayName('Where the Wonders of Learning Never Cease | Wonderopolis');
$resourceAdditionalData = [
	"link" => 'https://wonderopolis.org/',
	"thumbnailPreviewUrl" => null,
	"@odata.type" => '#microsoft.graph.educationLinkResource',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->resources()->post($requestRequestBody);


```