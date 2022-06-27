---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationalActivity();


$requestRequestBody->setCompletionMonthYear(new Date("Date"));
$requestRequestBody->setEndMonthYear(new Date("Date"));

$institution = new InstitutionData();
$requestRequestBody->setInstitution($institution);


$institution->setDescription(null);
$institution->setDisplayName('Colorado State University');

$location = new PhysicalAddress();
$institution->setLocation($location);


$location->setType(new PhysicalAddressType('business'));
$location->setPostOfficeBox(null);
$location->setStreet('12000 E Prospect Rd');
$location->setCity('Fort Collins');
$location->setState('Colorado');
$location->setCountryOrRegion('USA');
$location->setPostalCode('80525');

$institution->setWebUrl('https://www.colostate.edu');


$program = new EducationalActivityDetail();
$requestRequestBody->setProgram($program);


$program->setAbbreviation('MBA');
$program->setActivities(null);
$program->setAwards(null);
$program->setDescription('Master of Business Administration with a major in Entreprenuership and Finance.');
$program->setDisplayName('Master of Business Administration');
$program->setFieldsOfStudy(null);
$program->setGrade('3.9');
$program->setNotes(null);
$program->setWebUrl('https://biz.colostate.edu');

$requestRequestBody->setStartMonthYear(new Date("Date"));
$result =  $graphClient->me()->profile()->educationalActivities()->post($requestRequestBody);


```