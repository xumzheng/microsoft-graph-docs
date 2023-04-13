---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
additionalData = [
'allowedValues@delta' => allowed_values@delta1 = ()
		allowedValues@delta1.id = 'Baker'

		allowedValues@delta1.is_active = False


allowedValues@deltaArray []= allowedValues@delta1;
allowed_values@delta2 = ()
		allowedValues@delta2.id = 'Skagit'

		allowedValues@delta2.is_active = True


allowedValues@deltaArray []= allowedValues@delta2;
request_body.allowedvalues@delta(allowedValues@deltaArray)


];
request_body.additionaldata(additionalData)




request_configuration = CustomSecurityAttributeDefinitionRequestBuilder.CustomSecurityAttributeDefinitionRequestBuilderPatchRequestConfiguration(
headers = {
	'OData-Version' : "4.01",
}

)


result = await client.directory.customSecurityAttributeDefinitions_by_id('customSecurityAttributeDefinition-id').patch(request_body = request_body, request_configuration = request_configuration)


```