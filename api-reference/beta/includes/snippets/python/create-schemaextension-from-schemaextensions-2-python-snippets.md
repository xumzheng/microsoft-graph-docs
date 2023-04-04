---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SchemaExtension();
request_body.setId('courses');

request_body.setDescription('Graph Learn training courses extensions');

request_body.setTargetTypes(['Group', ]);

propertiesExtensionSchemaProperty1 = ExtensionSchemaProperty();
propertiesExtensionSchemaProperty1.setName('courseId');

propertiesExtensionSchemaProperty1.setType('Integer');


propertiesArray []= propertiesExtensionSchemaProperty1;
propertiesExtensionSchemaProperty2 = ExtensionSchemaProperty();
propertiesExtensionSchemaProperty2.setName('courseName');

propertiesExtensionSchemaProperty2.setType('String');


propertiesArray []= propertiesExtensionSchemaProperty2;
propertiesExtensionSchemaProperty3 = ExtensionSchemaProperty();
propertiesExtensionSchemaProperty3.setName('courseType');

propertiesExtensionSchemaProperty3.setType('String');


propertiesArray []= propertiesExtensionSchemaProperty3;
request_body.setProperties(propertiesArray);




result = await client.schemaExtensions().post(request_body);


```