---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = PeopleRequestBuilderGetRequestConfiguration();

queryParameters = PeopleRequestBuilderGetQueryParameters();
queryParameters.search = "\"Irene McGowen\"";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().people().get(requestConfiguration);


```