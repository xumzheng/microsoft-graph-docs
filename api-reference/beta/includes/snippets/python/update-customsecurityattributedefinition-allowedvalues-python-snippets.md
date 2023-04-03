---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CustomSecurityAttributeDefinition();
additionalData = [
'allowedValues@delta' => allowedValues@delta1 = ();
		allowedValues@delta1.setId('Baker');

		allowedValues@delta1.setIsActive(false);


allowedValues@deltaArray []= allowedValues@delta1;
allowedValues@delta2 = ();
		allowedValues@delta2.setId('Skagit');

		allowedValues@delta2.setIsActive(true);


allowedValues@deltaArray []= allowedValues@delta2;
requestBody.setAllowedValues@delta(allowedValues@deltaArray);


];
requestBody.setAdditionalData(additionalData);



request_config = CustomSecurityAttributeDefinitionRequestBuilderPatchRequestConfiguration();

headers = [
'OData-Version' => '4.01',
];

request_config.headers = headers;


result = await client.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').patch(requestBody, request_config);


```