---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CustodianSource();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/c25c3914-f9f7-43ee-9cba-a25377e0cec6', 
];
request_body.setAdditionalData(additionalData);




await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').searchesById('ediscoverySearch-id').custodianSourcesById('dataSource-id').post(request_body);


```