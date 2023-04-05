---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
additionalData = [
'allowedValues@delta' => allowedValues@delta1 = ()
		allowedValues@delta1.setId('Baker')

		allowedValues@delta1.setIsActive(false)


allowedValues@deltaArray []= allowedValues@delta1;
allowedValues@delta2 = ()
		allowedValues@delta2.setId('Skagit')

		allowedValues@delta2.setIsActive(true)


allowedValues@deltaArray []= allowedValues@delta2;
request_body.setAllowedValues@delta(allowedValues@deltaArray)


];
request_body.setAdditionalData(additionalData)



request_config = CustomSecurityAttributeDefinitionRequestBuilderPatchRequestConfiguration()

headers = [
'OData-Version' => '4.01',
]

request_config.headers = headers


result = await client.directory_customSecurityAttributeDefinitionsby_id('customSecurityAttributeDefinition-id').patch(request_body, request_config)


```