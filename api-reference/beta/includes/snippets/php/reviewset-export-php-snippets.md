---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExportPostRequestBody();


$requestRequestBody->setOutputName('2020-12-06 Contoso investigation export');
$requestRequestBody->setDescription('Export for the Contoso investigation');
$requestRequestBody->setExportOptions(new ExportOptions('originalFiles,fileInfo,tags'));
$requestRequestBody->setExportStructure(new ExportFileStructure('directory'));
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->reviewSetsById('reviewSet-id')->export()->post($requestRequestBody);


```