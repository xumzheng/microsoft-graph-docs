---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = $refDeleteRequestBody()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1.0/directoryObjects/{id}', 
];
request_body.setAdditionalData(additionalData)



request_config = RefRequestBuilderDeleteRequestConfiguration(
request_config = RefRequestBuilderDeleteRequestConfiguration(query_params=)


await client.servicePrincipals_by_id('servicePrincipal-id').owners_by_id('directoryObject-id').ref.delete(request_body, headers=)


```