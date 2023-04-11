---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition()
request_body.attributeSet = 'Engineering'

request_body.description = 'Active projects for user'

request_body.isCollection = true

request_body.isSearchable = true

request_body.name = 'Project'

request_body.status = 'Available'

request_body.type = 'String'

request_body.usePreDefinedValuesOnly = true

allowedValuesAllowedValue1 = AllowedValue()
allowedValuesAllowedValue1.id = 'Alpine'

allowedValuesAllowedValue1.isActive = true


allowedValuesArray []= allowedValuesAllowedValue1;
allowedValuesAllowedValue2 = AllowedValue()
allowedValuesAllowedValue2.id = 'Baker'

allowedValuesAllowedValue2.isActive = true


allowedValuesArray []= allowedValuesAllowedValue2;
allowedValuesAllowedValue3 = AllowedValue()
allowedValuesAllowedValue3.id = 'Cascade'

allowedValuesAllowedValue3.isActive = true


allowedValuesArray []= allowedValuesAllowedValue3;
request_body.allowedvalues(allowedValuesArray)




request_configuration = CustomSecurityAttributeDefinitionsRequestBuilderPostRequestConfiguration(
)


result = await client.directory.customSecurityAttributeDefinitions.post(request_body = request_body)


```