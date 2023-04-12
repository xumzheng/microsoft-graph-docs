---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchemaExtension()
request_body.owner = 'ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa'

propertiesExtensionSchemaProperty1 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty1.name = 'courseId'

propertiesExtensionSchemaProperty1.type = 'Integer'


propertiesArray []= propertiesExtensionSchemaProperty1;
propertiesExtensionSchemaProperty2 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty2.name = 'courseName'

propertiesExtensionSchemaProperty2.type = 'String'


propertiesArray []= propertiesExtensionSchemaProperty2;
propertiesExtensionSchemaProperty3 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty3.name = 'courseType'

propertiesExtensionSchemaProperty3.type = 'String'


propertiesArray []= propertiesExtensionSchemaProperty3;
propertiesExtensionSchemaProperty4 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty4.name = 'courseSupervisors'

propertiesExtensionSchemaProperty4.type = 'String'


propertiesArray []= propertiesExtensionSchemaProperty4;
request_body.properties(propertiesArray)





result = await client.schemaExtensions_by_id('schemaExtension-id').patch(request_body = request_body)


```