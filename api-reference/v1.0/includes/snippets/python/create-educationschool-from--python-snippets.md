---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EducationSchool();
$requestBody->set@odatatype('#microsoft.graph.educationSchool');

$requestBody->setDisplayName('String');

$requestBody->setDescription('String');

$requestBody->setExternalSource(new EducationExternalSource('string'));

$requestBody->setExternalSourceDetail('String');

$requestBody->setPrincipalEmail('String');

$requestBody->setPrincipalName('String');

$requestBody->setExternalPrincipalId('String');

$requestBody->setLowestGrade('String');

$requestBody->setHighestGrade('String');

$requestBody->setSchoolNumber('String');

$requestBody->setExternalId('String');

$requestBody->setPhone('String');

$requestBody->setFax('String');

$createdBy = new IdentitySet();
$createdBy->set@odatatype('microsoft.graph.identitySet');


$requestBody->setCreatedBy($createdBy);
$address = new PhysicalAddress();
$address->set@odatatype('microsoft.graph.physicalAddress');


$requestBody->setAddress($address);


$requestResult = $graphServiceClient->education()->schools()->post($requestBody);


```