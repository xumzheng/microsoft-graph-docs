---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ResourceConnection()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.operationalInsightsConnection')

additionalData = [
'azureSubscriptionId' => '322ec614-e9c2-4cd5-a55c-5711fdecf02e', 
'azureResourceGroupName' => 'target-resource-group', 
'workspaceName' => 'my-workspace', 
];
request_body.setAdditionalData(additionalData)




result = await client.admin_windows_updates_resourceConnections.post(request_body)


```