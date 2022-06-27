---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NoncustodialDataSource-idPostRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->sourceCollectionsById('sourceCollection-id')->noncustodialSourcesById('noncustodialDataSource-id')->post($requestRequestBody);


```