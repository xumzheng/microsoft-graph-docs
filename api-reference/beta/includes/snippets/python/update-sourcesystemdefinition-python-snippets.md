---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceSystemDefinition()
request_body.setVendor('LMS Vendor')


request_config = SourceSystemDefinitionRequestBuilderPatchRequestConfiguration(
request_config = SourceSystemDefinitionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.external.industryData.sourceSystems_by_id('sourceSystemDefinition-id').patch(request_body, headers=)


```