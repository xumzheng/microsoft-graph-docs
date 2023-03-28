---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ExportPostRequestBody();
$requestBody->setOutputName('2020-12-06 Contoso investigation export');

$requestBody->setDescription('Export for the Contoso investigation');

$requestBody->setExportOptions(new ExportOptions('originalfiles,fileinfo,tags'));

$requestBody->setExportStructure(new ExportFileStructure('directory'));



$graphServiceClient->compliance()->ediscovery()->casesById('case-id')->reviewSetsById('reviewSet-id')->ediscoveryExport()->post($requestBody);


```