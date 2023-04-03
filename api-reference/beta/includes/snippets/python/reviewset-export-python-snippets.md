---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ExportPostRequestBody();
requestBody.setOutputName('2020-12-06 Contoso investigation export');

requestBody.setDescription('Export for the Contoso investigation');

requestBody.setExportOptions(ExportOptions('originalfiles,fileinfo,tags'));

requestBody.setExportStructure(ExportFileStructure('directory'));



awaitclient.compliance().ediscovery().casesById('case-id').reviewSetsById('reviewSet-id').ediscoveryExport().post(requestBody);


```