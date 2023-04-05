---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AppConsentRequestRequestBuilderGetRequestConfiguration(
query_params = AppConsentRequestRequestBuilderGetQueryParameters()
query_params.filter = "userConsentRequests/any"

)


result = await client.identityGovernance.appConsent.appConsentRequests_by_id('appConsentRequest-id').get(request_config)


```