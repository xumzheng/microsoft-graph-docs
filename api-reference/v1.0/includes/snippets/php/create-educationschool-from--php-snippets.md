---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationSchool();


$requestRequestBody->setDisplayName('String');
$requestRequestBody->setDescription('String');
$requestRequestBody->setExternalSource(new EducationExternalSource('String'));
$requestRequestBody->setExternalSourceDetail('String');
$requestRequestBody->setPrincipalEmail('String');
$requestRequestBody->setPrincipalName('String');
$requestRequestBody->setExternalPrincipalId('String');
$requestRequestBody->setLowestGrade('String');
$requestRequestBody->setHighestGrade('String');
$requestRequestBody->setSchoolNumber('String');
$requestRequestBody->setExternalId('String');
$requestRequestBody->setPhone('String');
$requestRequestBody->setFax('String');

$createdBy = new IdentitySet();
$requestRequestBody->setCreatedBy($createdBy);


$createdByAdditionalData = [
	"@odata.type" => 'microsoft.graph.identitySet',
];
$createdBy->setAdditionalData($createdByAdditionalData);


$address = new PhysicalAddress();
$requestRequestBody->setAddress($address);


$addressAdditionalData = [
"@odata.type" => 'microsoft.graph.physicalAddress',
];
$address->setAdditionalData($addressAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.educationSchool',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->education()->schools()->post($requestRequestBody);


```