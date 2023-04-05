---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPostRequestBody()
request_body.setOutputName('2020-12-06 Contoso investigation export')

request_body.setDescription('Export for the Contoso investigation')

request_body.setExportOptions(ExportOptions('originalfiles,fileinfo,tags'))

request_body.setExportStructure(ExportFileStructure('directory'))



await client.compliance.ediscovery.casesById('case-id').reviewSetsById('reviewSet-id').ediscoveryexport.post(request_body)


```