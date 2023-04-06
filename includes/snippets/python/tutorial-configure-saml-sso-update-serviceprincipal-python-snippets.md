---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ServicePrincipal()
request_body.setPreferredSingleSignOnMode('saml')


request_config = ServicePrincipalRequestBuilderPatchRequestConfiguration(
request_config = ServicePrincipalRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.servicePrincipals_by_id('servicePrincipal-id').patch(request_body, headers=)


```