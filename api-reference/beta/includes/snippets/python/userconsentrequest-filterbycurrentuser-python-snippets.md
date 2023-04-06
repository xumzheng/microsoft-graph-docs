---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UserConsentRequestRequestBuilderGetRequestConfiguration(
request_configuration = UserConsentRequestRequestBuilderGetRequestConfiguration(query_params=query_params = UserConsentRequestRequestBuilderGetQueryParameters()
query_params['filter'] = " "

)
query_params = UserConsentRequestRequestBuilderGetQueryParameters()
query_params['filter'] = " "

)


result = await client.identityGovernance.appConsent.appConsentRequests_by_id('appConsentRequest-id').userConsentRequests_by_id('userConsentRequest-id').get(request_configuration)


```