---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EducationalActivity();
$institution = new InstitutionData();
$institutionLocation = new PhysicalAddress();
$institutionLocation->setType(new PhysicalAddressType('business'));

$InstitutionLocation->setPostOfficeBox(null);

$institutionLocation->setStreet('12000 E Prospect Rd');

$institutionLocation->setCity('Fort Collins');

$institutionLocation->setState('Colorado');

$institutionLocation->setCountryOrRegion('USA');

$institutionLocation->setPostalCode('80525');


$institution->setLocation($institutionLocation);

$requestBody->setInstitution($institution);


$requestResult = $graphServiceClient->me()->profile()->educationalActivitiesById('educationalActivity-id')->patch($requestBody);


```