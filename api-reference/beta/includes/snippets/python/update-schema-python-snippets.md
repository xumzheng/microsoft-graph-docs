---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Schema();
requestBody.setBaseType('microsoft.graph.externalItem');

propertiesProperty1 = Property();
propertiesProperty1.setName('ticketTitle');

propertiesProperty1.setType(PropertyType('string'));

propertiesProperty1.setIsSearchable(true);

propertiesProperty1.setIsRetrievable(true);

propertiesProperty1.setLabels([propertiesProperty1.setLabel(Label('title'));
]);


propertiesArray []= propertiesProperty1;
propertiesProperty2 = Property();
propertiesProperty2.setName('priority');

propertiesProperty2.setType(PropertyType('string'));

propertiesProperty2.setIsQueryable(true);

propertiesProperty2.setIsRetrievable(true);

propertiesProperty2.setIsSearchable(false);


propertiesArray []= propertiesProperty2;
propertiesProperty3 = Property();
propertiesProperty3.setName('assignee');

propertiesProperty3.setType(PropertyType('string'));

propertiesProperty3.setIsRetrievable(true);


propertiesArray []= propertiesProperty3;
requestBody.setProperties(propertiesArray);




result = awaitclient.external().connectionsById('externalConnection-id').schema().patch(requestBody);


```