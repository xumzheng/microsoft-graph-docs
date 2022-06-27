---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationUser();


$requestRequestBody->setDisplayName('Dion Matheson');
$requestRequestBody->setGivenName('Dion');
$requestRequestBody->setMiddleName(null);
$requestRequestBody->setSurname('Matheson');
$requestRequestBody->setMail('DionM@contoso.com');
$requestRequestBody->setMobilePhone('+1 (253) 555-0101');

$createdBy = new IdentitySet();
$requestRequestBody->setCreatedBy($createdBy);



$user = new Identity();
$createdBy->setUser($user);


$user->setDisplayName('Susana Rocha');
$user->setId('14012');


$requestRequestBody->setExternalSource(new EducationExternalSource('sis'));

$mailingAddress = new PhysicalAddress();
$requestRequestBody->setMailingAddress($mailingAddress);


$mailingAddress->setCity('Los Angeles');
$mailingAddress->setCountryOrRegion('United States');
$mailingAddress->setPostalCode('98055');
$mailingAddress->setState('CA');
$mailingAddress->setStreet('12345 Main St.');

$requestRequestBody->setPrimaryRole(new EducationUserRole('student'));

$residenceAddress = new PhysicalAddress();
$requestRequestBody->setResidenceAddress($residenceAddress);


$residenceAddress->setCity('Los Angeles');
$residenceAddress->setCountryOrRegion('United States');
$residenceAddress->setPostalCode('98055');
$residenceAddress->setState('CA');
$residenceAddress->setStreet('12345 Main St.');

$result =  $graphClient->education()->users()->post($requestRequestBody);


```