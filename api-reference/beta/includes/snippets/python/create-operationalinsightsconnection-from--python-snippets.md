---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ResourceConnection();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.operationalInsightsConnection');

additionalData = [
'azureSubscriptionId' => '322ec614-e9c2-4cd5-a55c-5711fdecf02e', 
'azureResourceGroupName' => 'target-resource-group', 
'workspaceName' => 'my-workspace', 
];
requestBody.setAdditionalData(additionalData);




result = await client.admin().windows().updates().resourceConnections().post(requestBody);


```