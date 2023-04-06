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



request_configuration = SynchronizationTemplateRequestBuilderPutRequestConfiguration(
request_configuration = SynchronizationTemplateRequestBuilderPutRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


await client.applications_by_id('application-id').synchronization.templates_by_id('synchronizationTemplate-id').put(request_body, request_configuration)


```