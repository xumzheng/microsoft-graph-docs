---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchemaExtension()
request_body.setOwner('ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa')

propertiesExtensionSchemaProperty1 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty1.setName('courseId')

propertiesExtensionSchemaProperty1.setType('Integer')


propertiesArray []= propertiesExtensionSchemaProperty1;
propertiesExtensionSchemaProperty2 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty2.setName('courseName')

propertiesExtensionSchemaProperty2.setType('String')


propertiesArray []= propertiesExtensionSchemaProperty2;
propertiesExtensionSchemaProperty3 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty3.setName('courseType')

propertiesExtensionSchemaProperty3.setType('String')


propertiesArray []= propertiesExtensionSchemaProperty3;
propertiesExtensionSchemaProperty4 = ExtensionSchemaProperty()
propertiesExtensionSchemaProperty4.setName('courseSupervisors')

propertiesExtensionSchemaProperty4.setType('String')


propertiesArray []= propertiesExtensionSchemaProperty4;
request_body.setProperties(propertiesArray)




result = await client.schemaExtensionsById('schemaExtension-id').patch(request_body)


```