---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SubjectRightsRequest();


$requestRequestBody->setType(new SubjectRightsRequestType('export'));
$requestRequestBody->setContentQuery('(("Diego Siciliani" OR "Diego.Siciliani@contoso.com") OR (participants:"Diego.Siciliani@contoso.com"))');
$requestRequestBody->setDataSubjectType(new DataSubjectType('customer'));
$requestRequestBody->setExternalId('F53BF2DA-607D-412A-B568-FAA0F023AC0B');
$requestRequestBody->setDisplayName('Export report for customer Id: 12345');
$requestRequestBody->setDescription('This is a export request');
$requestRequestBody->setIncludeAllVersions(False);
$requestRequestBody->setIncludeAuthoredContent(True);
$requestRequestBody->setInternalDueDateTime(new DateTime("2022-07-20T22:42:28Z"));

$dataSubject = new DataSubject();
$requestRequestBody->setDataSubject($dataSubject);


$dataSubject->setFirstName('Diego');
$dataSubject->setLastName('Siciliani');
$dataSubject->setEmail('Diego.Siciliani@contoso.com');
$dataSubject->setResidency('USA');

$requestRequestBody->setMailboxLocations(null);
$requestRequestBody->setPauseAfterEstimate(True);
$requestRequestBody->setRegulations( [
'CCPA',],

$siteLocations = new SubjectRightsRequestSiteLocation();
$requestRequestBody->setSiteLocations($siteLocations);


$siteLocationsAdditionalData = [
"@odata.type" => 'microsoft.graph.subjectRightsRequestAllSiteLocation',
];
$siteLocations->setAdditionalData($siteLocationsAdditionalData);

$result =  $graphClient->privacy()->subjectRightsRequests()->post($requestRequestBody);


```