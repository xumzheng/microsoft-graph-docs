---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = Oauth2PermissionGrantsRequestBuilderGetRequestConfiguration(
request_configuration = Oauth2PermissionGrantsRequestBuilderGetRequestConfiguration(query_params=query_params = Oauth2PermissionGrantsRequestBuilderGetQueryParameters()
query_params['filter'] = "clientId eq 'b0d9b9e3-0ecf-4bfd-8dab-9273dd055a94' and principalId eq '3fbd929d-8c56-4462-851e-0eb9a7b3a2a5' and consentType eq 'Principal'"

)
query_params = Oauth2PermissionGrantsRequestBuilderGetQueryParameters()
query_params['filter'] = "clientId eq 'b0d9b9e3-0ecf-4bfd-8dab-9273dd055a94' and principalId eq '3fbd929d-8c56-4462-851e-0eb9a7b3a2a5' and consentType eq 'Principal'"

)


result = await client.oauth2PermissionGrants.get(request_configuration)


```