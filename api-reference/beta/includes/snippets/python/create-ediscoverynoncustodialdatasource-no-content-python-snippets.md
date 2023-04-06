---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NoncustodialSource()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339', 
];
request_body.setAdditionalData(additionalData)




await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').searches_by_id('ediscoverySearch-id').noncustodialSources_by_id('ediscoveryNoncustodialDataSource-id').post(request_body, headers=)


```