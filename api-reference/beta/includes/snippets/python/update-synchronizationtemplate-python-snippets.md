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
request_body.additionaldata(additionalData)




request_configuration = SynchronizationTemplateRequestBuilder.SynchronizationTemplateRequestBuilderPutRequestConfiguration(
headers = {
		'Authorization' : "Bearer <token>",
}

)


await client.applications_by_id('application-id').synchronization.templates_by_id('synchronizationTemplate-id').put(request_body = request_body, request_configuration = request_configuration)


```