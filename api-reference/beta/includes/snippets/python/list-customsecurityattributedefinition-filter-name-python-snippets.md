---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration();

query_params = CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters();
query_params.filter = "name eq 'Project' and status eq 'Available'";

request_config.queryParameters = query_params;


result = await client.directory.customSecurityAttributeDefinitions.get(request_config);


```