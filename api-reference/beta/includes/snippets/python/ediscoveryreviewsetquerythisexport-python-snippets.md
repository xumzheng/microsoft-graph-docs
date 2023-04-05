---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPostRequestBody()
request_body.setOutputName('Export reviewset query via API')

request_body.setDescription('Export for the Contoso investigation 2')

request_body.setExportOptions(ExportOptions('originalfiles,fileinfo,tags'))

request_body.setExportStructure(ExportFileStructure('directory'))



await client.security.cases.ediscoveryCasesby_id('ediscoveryCase-id').reviewSetsby_id('ediscoveryReviewSet-id').queriesby_id('ediscoveryReviewSetQuery-id').securityexport.post(request_body)


```