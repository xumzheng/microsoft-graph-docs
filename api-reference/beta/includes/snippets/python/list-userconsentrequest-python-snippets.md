---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = UserConsentRequestsRequestBuilderGetRequestConfiguration(
)


result = await client.identityGovernance.appConsent.appConsentRequests_by_id('appConsentRequest-id').userConsentRequests.get()


```