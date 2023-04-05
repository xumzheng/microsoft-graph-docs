---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Template()
additionalData = [
'id' => 'Slack', 
'applicationId' => '{id}', 
'factoryTag' => 'CustomSCIM', 
];
request_body.setAdditionalData(additionalData)



request_config = SynchronizationTemplateRequestBuilderPutRequestConfiguration()

headers = [
	'Authorization' => 'Bearer <token>',
]

request_config.headers = headers


await client.applicationsById('application-id').synchronization.templatesById('synchronizationTemplate-id').put(request_body, request_config)


```