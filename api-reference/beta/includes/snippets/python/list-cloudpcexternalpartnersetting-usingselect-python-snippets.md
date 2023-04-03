---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ExternalPartnerSettingsRequestBuilderGetRequestConfiguration();

query_params = ExternalPartnerSettingsRequestBuilderGetQueryParameters();
query_params.select = ["id","partnerId","enableConnection"];

request_config.queryParameters = query_params;


result = awaitclient.deviceManagement().virtualEndpoint().externalPartnerSettings().get(request_config);


```