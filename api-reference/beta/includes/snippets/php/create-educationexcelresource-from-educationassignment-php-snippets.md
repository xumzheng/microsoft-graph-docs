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


$resource->setDisplayName('Graph Doc pages.xlsx');
$resourceAdditionalData = [
	"@odata.type" => 'microsoft.graph.educationExcelResource',
	"fileUrl" => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2',
];
$resource->setAdditionalData($resourceAdditionalData);

$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->resources()->post($requestRequestBody);


```