---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NoncustodialDataSource();


$requestRequestBody->setApplyHoldToSource(False);

$dataSource = new DataSource();
$requestRequestBody->setDataSource($dataSource);


$dataSourceAdditionalData = [
	"@odata.type" => 'microsoft.graph.ediscovery.siteSource',
];
$dataSource->setAdditionalData($dataSourceAdditionalData);

$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->noncustodialDataSources()->post($requestRequestBody);


```