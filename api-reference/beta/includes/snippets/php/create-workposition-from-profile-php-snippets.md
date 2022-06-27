---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new WorkPosition();



$detail = new PositionDetail();
$requestRequestBody->setDetail($detail);



$company = new CompanyDetail();
$detail->setCompany($company);


$company->setDisplayName('Adventureworks Ltd.');
$company->setDepartment('Consulting');
$company->setOfficeLocation('AW23/344');

$address = new PhysicalAddress();
$company->setAddress($address);


$address->setType(new PhysicalAddressType('business'));
$address->setStreet('123 Patriachy Ponds');
$address->setCity('Moscow');
$address->setCountryOrRegion('Russian Federation');
$address->setPostalCode('RU-34621');

$company->setWebUrl('https://www.adventureworks.com');

$detail->setJobTitle('Senior Product Branding Manager II');
$detail->setRole('consulting');

$requestRequestBody->setIsCurrent(True);
$result =  $graphClient->me()->profile()->positions()->post($requestRequestBody);


```