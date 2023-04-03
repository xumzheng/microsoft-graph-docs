---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ExportPostRequestBody();
requestBody.setOutputName('Export reviewset query via API');

requestBody.setDescription('Export for the Contoso investigation 2');

requestBody.setExportOptions(ExportOptions('originalfiles,fileinfo,tags'));

requestBody.setExportStructure(ExportFileStructure('directory'));



await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSetsById('ediscoveryReviewSet-id').queriesById('ediscoveryReviewSetQuery-id').securityExport().post(requestBody);


```