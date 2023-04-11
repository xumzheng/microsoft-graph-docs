---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPostRequestBody()
request_body.outputName = 'Export via API'

request_body.description = 'Export for the Contoso investigation'

request_body.ExportOptions(ExportOptions('originalfiles,fileinfo,tags'))

request_body.ExportStructure(ExportFileStructure('directory'))




await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').reviewSets_by_id('ediscoveryReviewSet-id').securityexport.post(request_body = request_body)


```