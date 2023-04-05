---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchemaPostRequestBody()
additionalData = [
'baseType' => 'microsoft.graph.externalItem', 
'properties' => properties1 = ()
		properties1.setName('ticketTitle')

		properties1.setType('string')

		properties1.setIsSearchable('true')

		properties1.setIsRetrievable('true')

properties1.setLabels(['title', ])


propertiesArray []= properties1;
properties2 = ()
	properties2.setName('priority')

	properties2.setType('string')

	properties2.setIsQueryable('true')

	properties2.setIsRetrievable('true')

	properties2.setIsSearchable('false')


propertiesArray []= properties2;
properties3 = ()
	properties3.setName('assignee')

	properties3.setType('string')

	properties3.setIsRetrievable('true')


propertiesArray []= properties3;
request_body.setProperties(propertiesArray)


];
request_body.setAdditionalData(additionalData)




await client.external_connectionsby_id('externalConnection-id')_schema.post(request_body)


```