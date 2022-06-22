---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SitePage();


$requestRequestBody->setName('Events.aspx');
$requestRequestBody->setTitle('Team Events');

$publishingState = new PublicationFacet();
$requestRequestBody->setPublishingState($publishingState);


$publishingState->setLevel('checkedOut');
$publishingState->setVersionId('0.1');

$webPartsArray = [];

$webParts1 = new WebPart();

$webParts1->setType('rte');

$data = new SitePageData();
$webParts1->setData($data);


$dataAdditionalData = [
	"innerHTML" => '<p>Here are the team\'s upcoming events:</p>',
];
$data->setAdditionalData($dataAdditionalData);


$webPartsArray []= $webParts1;

$webParts2 = new WebPart();

$webParts2->setType('d1d91016-032f-456d-98a4-721247c305e8');

$data = new SitePageData();
$webParts2->setData($data);


$dataAdditionalData = [
"title" => 'Events',
"description" => 'Display upcoming events',
"dataVersion" => '1.0',
];
$data->setAdditionalData($dataAdditionalData);


$webPartsArray []= $webParts2;
$requestRequestBody->setWebParts($webPartsArray);
$result =  $graphClient->sitesById('site-id')->pages()->post($requestRequestBody);


```