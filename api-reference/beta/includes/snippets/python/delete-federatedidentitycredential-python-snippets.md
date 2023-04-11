---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = FederatedIdentityCredentialRequestBuilderDeleteRequestConfiguration(
)


await client.applications_by_id('application-id').federatedIdentityCredentials_by_id('federatedIdentityCredential-id').delete()


```