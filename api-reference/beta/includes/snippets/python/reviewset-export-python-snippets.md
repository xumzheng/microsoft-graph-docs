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



await client.compliance_ediscovery_casesby_id('case-id')_reviewSetsby_id('reviewSet-id')_ediscoveryexport.post(request_body)


```