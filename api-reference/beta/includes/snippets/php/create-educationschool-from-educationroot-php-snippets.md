---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationSchool();


$requestRequestBody->setDisplayName('Fabrikam High School');
$requestRequestBody->setDescription('Magnate school for the arts. Los Angeles School District');
$requestRequestBody->setExternalSource(new EducationExternalSource('String'));
$requestRequestBody->setPrincipalEmail('AmyR@fabrikam.com');
$requestRequestBody->setPrincipalName('Amy Roebuck');
$requestRequestBody->setExternalPrincipalId('14007');
$requestRequestBody->setHighestGrade('12');
$requestRequestBody->setLowestGrade('9');
$requestRequestBody->setSchoolNumber('10002');

$address = new PhysicalAddress();
$requestRequestBody->setAddress($address);


$address->setCity('Los Angeles');
$address->setCountryOrRegion('United States');
$address->setPostalCode('98055');
$address->setState('CA');
$address->setStreet('12345 Main St.');

$requestRequestBody->setExternalId('10002');
$requestRequestBody->setPhone('+1 (253) 555-0102');
$result =  $graphClient->education()->schools()->post($requestRequestBody);


```