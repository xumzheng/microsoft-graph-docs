---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPostRequestBody()
request_body.setOutputName('Export via API')

request_body.setDescription('Export for the Contoso investigation')

request_body.setExportOptions(ExportOptions('originalfiles,fileinfo,tags'))

request_body.setExportStructure(ExportFileStructure('directory'))



await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_reviewSetsby_id('ediscoveryReviewSet-id')_securityexport.post(request_body)


```