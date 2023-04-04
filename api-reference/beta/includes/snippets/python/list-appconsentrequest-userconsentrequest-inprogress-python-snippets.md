---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AppConsentRequestsRequestBuilderGetRequestConfiguration();

query_params = AppConsentRequestsRequestBuilderGetQueryParameters;
query_params.filter = "userConsentRequests/any ";

request_config.queryParameters = query_params;


result = await client.identityGovernance().appConsent().appConsentRequests().get(request_config);


```