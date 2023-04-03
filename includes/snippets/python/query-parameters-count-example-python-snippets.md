---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ContactsRequestBuilderGetRequestConfiguration();

queryParameters = ContactsRequestBuilderGetQueryParameters();
queryParameters.count = true;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().contacts().get(requestConfiguration);


```