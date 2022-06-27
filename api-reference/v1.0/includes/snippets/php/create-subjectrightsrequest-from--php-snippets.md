---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SubjectRightsRequest();


$requestRequestBody->setType(new SubjectRightsRequestType('microsoft.graph.subjectRightsRequestType'));
$requestRequestBody->setDataSubjectType(new DataSubjectType('microsoft.graph.dataSubjectType'));
$requestRequestBody->setRegulations(['String',]);
$requestRequestBody->setDisplayName('String');
$requestRequestBody->setDescription('String');
$requestRequestBody->setInternalDueDateTime(new DateTime("String (timestamp)"));

$dataSubject = new DataSubject();
$requestRequestBody->setDataSubject($dataSubject);


$dataSubject->setFirstName('String');
$dataSubject->setLastName('String');
$dataSubject->setEmail('String');
$dataSubject->setResidency('String');
$dataSubjectAdditionalData = [
"phoneNumber" => 'String',
"SSN" => 'String',
];
$dataSubject->setAdditionalData($dataSubjectAdditionalData);

$result =  $graphClient->privacy()->subjectRightsRequests()->post($requestRequestBody);


```