---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ApplicationTemplatesRequestBuilderGetRequestConfiguration();

query_params = ApplicationTemplatesRequestBuilderGetQueryParameters();
query_params.filter = "displayName eq 'AWS IAM Identity Center '";

request_config.queryParameters = query_params;


result = awaitclient.applicationTemplates().get(request_config);


```