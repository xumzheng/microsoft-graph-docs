---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ContactsRequestBuilderGetRequestConfiguration();

queryParameters = ContactsRequestBuilderGetQueryParameters();
queryParameters.search = "\"displayName:wa\"";
queryParameters.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.contacts().get(requestConfiguration);


```