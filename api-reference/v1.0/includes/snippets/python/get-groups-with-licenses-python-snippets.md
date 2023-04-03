---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = GroupsRequestBuilderGetRequestConfiguration();

queryParameters = GroupsRequestBuilderGetQueryParameters();
queryParameters.select = ["id","assignedLicenses"];
queryParameters.filter = "assignedLicenses/any()";
queryParameters.expand = ["members($select=id,displayName)"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.groups().get(requestConfiguration);


```