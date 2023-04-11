---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RefRequestBuilderDeleteRequestConfiguration(
)


await client.servicePrincipals_by_id('servicePrincipal-id').homeRealmDiscoveryPolicies_by_id('homeRealmDiscoveryPolicy-id').ref.delete()


```