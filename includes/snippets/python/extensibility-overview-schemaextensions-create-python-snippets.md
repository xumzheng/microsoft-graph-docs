---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SchemaExtension();
requestBody.setId('graphLearnCourses');

requestBody.setDescription('Graph Learn training courses extensions');

requestBody.setTargetTypes(['user', ]);

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
requestBody.setProperties(propertiesArray);




result = await client.schemaExtensions().post(requestBody);


```