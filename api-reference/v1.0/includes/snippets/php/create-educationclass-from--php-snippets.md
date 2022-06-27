---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationClass();


$requestRequestBody->setDisplayName('String');
$requestRequestBody->setMailNickname('String');
$requestRequestBody->setDescription('String');

$createdBy = new IdentitySet();
$requestRequestBody->setCreatedBy($createdBy);


$createdByAdditionalData = [
	"@odata.type" => 'microsoft.graph.identitySet',
];
$createdBy->setAdditionalData($createdByAdditionalData);

$requestRequestBody->setClassCode('String');
$requestRequestBody->setExternalName('String');
$requestRequestBody->setExternalId('String');
$requestRequestBody->setExternalSource(new EducationExternalSource('String'));
$requestRequestBody->setExternalSourceDetail('String');
$requestRequestBody->setGrade('String');

$term = new EducationTerm();
$requestRequestBody->setTerm($term);


$termAdditionalData = [
"@odata.type" => 'microsoft.graph.educationTerm',
];
$term->setAdditionalData($termAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.educationClass',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->education()->classes()->post($requestRequestBody);


```