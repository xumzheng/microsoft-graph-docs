---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SubjectRightsRequest();
$requestBody->setType(new SubjectRightsRequestType('subjectrightsrequesttype'));

$requestBody->setDataSubjectType(new DataSubjectType('datasubjecttype'));

$requestBody->setRegulations(['String', ]);

$requestBody->setDisplayName('String');

$requestBody->setDescription('String');

$requestBody->setInternalDueDateTime(new DateTime('String (timestamp)'));

$dataSubject = new DataSubject();
$dataSubject->setFirstName('String');

$dataSubject->setLastName('String');

$dataSubject->setEmail('String');

$dataSubject->setResidency('String');

$additionalData = [
'phoneNumber' => 'String', 
'SSN' => 'String', 
];
$dataSubject->setAdditionalData($additionalData);



$requestBody->setDataSubject($dataSubject);


$requestResult = $graphServiceClient->privacy()->subjectRightsRequests()->post($requestBody);


```