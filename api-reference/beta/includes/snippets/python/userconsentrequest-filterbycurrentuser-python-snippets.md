---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = UserConsentRequestRequestBuilderGetRequestConfiguration()

query_params = UserConsentRequestRequestBuilderGetQueryParameters()
query_params.filter = " "

request_config.queryParameters = query_params


result = await client.identityGovernance.appConsent.appConsentRequestsById('appConsentRequest-id').userConsentRequestsById('userConsentRequest-id').get(request_config)


```