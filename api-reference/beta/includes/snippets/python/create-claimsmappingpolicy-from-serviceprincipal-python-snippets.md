---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReferenceCreate();
request_body.set@odataid('https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9');



await client.servicePrincipalsById('servicePrincipal-id').claimsMappingPolicies.ref.post(request_body);


```