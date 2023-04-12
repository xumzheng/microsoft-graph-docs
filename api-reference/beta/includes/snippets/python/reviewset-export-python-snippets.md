---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPostRequestBody()
request_body.outputName = '2020-12-06 Contoso investigation export'

request_body.description = 'Export for the Contoso investigation'

request_body.ExportOptions(ExportOptions('originalfiles,fileinfo,tags'))

request_body.ExportStructure(ExportFileStructure('directory'))




await client.compliance.ediscovery.cases_by_id('case-id').reviewSets_by_id('reviewSet-id').ediscoveryexport.post(request_body = request_body)


```