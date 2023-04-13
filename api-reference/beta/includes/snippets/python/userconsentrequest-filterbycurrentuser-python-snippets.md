---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UserConsentRequestRequestBuilder.UserConsentRequestRequestBuilderGetQueryParameters(
		filter = " ",
)

request_configuration = UserConsentRequestRequestBuilder.UserConsentRequestRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.appConsent.appConsentRequests_by_id('appConsentRequest-id').userConsentRequests_by_id('userConsentRequest-id').get(request_configuration = request_configuration)


```