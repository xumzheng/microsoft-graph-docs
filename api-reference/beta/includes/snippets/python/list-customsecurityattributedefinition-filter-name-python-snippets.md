---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration();

queryParameters = CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters();
queryParameters.filter = "name eq 'Project' and status eq 'Available'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.directory().customSecurityAttributeDefinitions().get(requestConfiguration);


```