---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExtensionProperty()
request_body.setName('jobGroup')

request_body.setDataType('String')

request_body.setTargetObjects(['User', ])


request_config = ExtensionPropertiesRequestBuilderPostRequestConfiguration(
request_config = ExtensionPropertiesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.applications_by_id('application-id').extensionProperties.post(request_body, headers=)


```