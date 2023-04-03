---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CustomSecurityAttributeDefinition();
requestBody.setAttributeSet('Engineering');

requestBody.setDescription('Active projects for user');

requestBody.setIsCollection(true);

requestBody.setIsSearchable(true);

requestBody.setName('Project');

requestBody.setStatus('Available');

requestBody.setType('String');

requestBody.setUsePreDefinedValuesOnly(true);

allowedValuesAllowedValue1 = AllowedValue();
allowedValuesAllowedValue1.setId('Alpine');

allowedValuesAllowedValue1.setIsActive(true);


allowedValuesArray []= allowedValuesAllowedValue1;
allowedValuesAllowedValue2 = AllowedValue();
allowedValuesAllowedValue2.setId('Baker');

allowedValuesAllowedValue2.setIsActive(true);


allowedValuesArray []= allowedValuesAllowedValue2;
allowedValuesAllowedValue3 = AllowedValue();
allowedValuesAllowedValue3.setId('Cascade');

allowedValuesAllowedValue3.setIsActive(true);


allowedValuesArray []= allowedValuesAllowedValue3;
requestBody.setAllowedValues(allowedValuesArray);




result = awaitclient.directory().customSecurityAttributeDefinitions().post(requestBody);


```