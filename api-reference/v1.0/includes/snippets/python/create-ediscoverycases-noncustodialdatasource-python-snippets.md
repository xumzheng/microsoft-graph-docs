---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = NoncustodialSource();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339', 
];
requestBody.setAdditionalData(additionalData);




graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').searchesById('ediscoverySearch-id').noncustodialSourcesById('ediscoveryNoncustodialDataSource-id').post(requestBody);


```