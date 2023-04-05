---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
request_body.setAttributeSet('Engineering')

request_body.setDescription('Active projects for user')

request_body.setIsCollection(true)

request_body.setIsSearchable(true)

request_body.setName('Project')

request_body.setStatus('Available')

request_body.setType('String')

request_body.setUsePreDefinedValuesOnly(true)

allowedValuesAllowedValue1 = AllowedValue()
allowedValuesAllowedValue1.setId('Alpine')

allowedValuesAllowedValue1.setIsActive(true)


allowedValuesArray []= allowedValuesAllowedValue1;
allowedValuesAllowedValue2 = AllowedValue()
allowedValuesAllowedValue2.setId('Baker')

allowedValuesAllowedValue2.setIsActive(true)


allowedValuesArray []= allowedValuesAllowedValue2;
allowedValuesAllowedValue3 = AllowedValue()
allowedValuesAllowedValue3.setId('Cascade')

allowedValuesAllowedValue3.setIsActive(true)


allowedValuesArray []= allowedValuesAllowedValue3;
request_body.setAllowedValues(allowedValuesArray)




result = await client.directory_customSecurityAttributeDefinitions.post(request_body)


```