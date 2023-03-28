---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ExportPostRequestBody();
$requestBody.setOutputName('Export reviewset query via API');

$requestBody.setDescription('Export for the Contoso investigation 2');

$requestBody.setExportOptions(new ExportOptions('originalfiles,fileinfo,tags'));

$requestBody.setExportStructure(new ExportFileStructure('directory'));



$graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSetsById('ediscoveryReviewSet-id').queriesById('ediscoveryReviewSetQuery-id').securityExport().post($requestBody);


```