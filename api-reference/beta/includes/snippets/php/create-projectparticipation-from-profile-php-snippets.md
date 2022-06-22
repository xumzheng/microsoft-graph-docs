---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ProjectParticipation();


$requestRequestBody->setCategories( [
'Branding',],

$client = new CompanyDetail();
$requestRequestBody->setClient($client);


$client->setDisplayName('Contoso Ltd.');
$client->setDepartment('Corporate Marketing');
$client->setWebUrl('https://www.contoso.com');

$requestRequestBody->setDisplayName('Contoso Re-branding Project');

$detail = new PositionDetail();
$requestRequestBody->setDetail($detail);



$company = new CompanyDetail();
$detail->setCompany($company);


$company->setDisplayName('Adventureworks Inc.');
$company->setDepartment('Consulting');
$company->setWebUrl('https://adventureworks.com');

$detail->setDescription('Rebranding of Contoso Ltd.');
$detail->setJobTitle('Lead PM Rebranding');
$detail->setRole('project management');
$detail->setSummary('A 6 month project to help Contoso rebrand after they were divested from a parent organization.');

$result =  $graphClient->me()->profile()->projects()->post($requestRequestBody);


```