---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

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



requestConfiguration = CustomSecurityAttributeDefinitionRequestBuilderPatchRequestConfiguration();

headers = [
'OData-Version' => '4.01',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').patch(requestBody, requestConfiguration);


```