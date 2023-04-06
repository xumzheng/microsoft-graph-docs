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



request_config = SynchronizationTemplateRequestBuilderPutRequestConfiguration(
request_config = SynchronizationTemplateRequestBuilderPutRequestConfiguration(query_params=)
headers['Authorization'] = "Bearer <token>"


await client.applications_by_id('application-id').synchronization.templates_by_id('synchronizationTemplate-id').put(request_body, request_config, headers=request_config)


```