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
		properties1.name = 'ticketTitle'

		properties1.type = 'string'

		properties1.isSearchable = 'true'

		properties1.isRetrievable = 'true'

properties1.Labels(['title', ])


propertiesArray []= properties1;
properties2 = ()
	properties2.name = 'priority'

	properties2.type = 'string'

	properties2.isQueryable = 'true'

	properties2.isRetrievable = 'true'

	properties2.isSearchable = 'false'


propertiesArray []= properties2;
properties3 = ()
	properties3.name = 'assignee'

	properties3.type = 'string'

	properties3.isRetrievable = 'true'


propertiesArray []= properties3;
request_body.properties(propertiesArray)


];
request_body.additionaldata(additionalData)




request_configuration = SchemaRequestBuilderPostRequestConfiguration(
)


await client.external.connections_by_id('externalConnection-id').schema.post(request_body = request_body)


```