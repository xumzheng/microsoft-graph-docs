---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AppConsentRequestRequestBuilder.AppConsentRequestRequestBuilderGetQueryParameters(
		filter = "userConsentRequests/any",
)

request_configuration = AppConsentRequestRequestBuilder.AppConsentRequestRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.appConsent.appConsentRequests_by_id('appConsentRequest-id').get(request_configuration = request_configuration)


```