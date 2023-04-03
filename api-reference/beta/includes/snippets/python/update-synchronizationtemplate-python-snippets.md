---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Template();
additionalData = [
'id' => 'Slack', 
'applicationId' => '{id}', 
'factoryTag' => 'CustomSCIM', 
];
requestBody.setAdditionalData(additionalData);



requestConfiguration = SynchronizationTemplateRequestBuilderPutRequestConfiguration();

headers = [
	'Authorization' => 'Bearer <token>',
];

requestConfiguration.headers = headers;


graphServiceClient.applicationsById('application-id').synchronization().templatesById('synchronizationTemplate-id').put(requestBody, requestConfiguration);


```