---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
request_body.setDescription('Target completion date (YYYY/MM/DD)')


request_config = CustomSecurityAttributeDefinitionRequestBuilderPatchRequestConfiguration(
request_config = CustomSecurityAttributeDefinitionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.directory.customSecurityAttributeDefinitions_by_id('customSecurityAttributeDefinition-id').patch(request_body, headers=)


```