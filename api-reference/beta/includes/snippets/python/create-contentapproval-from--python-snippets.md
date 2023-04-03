---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ComplianceChange();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.contentApproval');

additionalData = [
'content' => requestBody = Content();
		requestBody.set@odatatype('#microsoft.graph.windowsUpdates.catalogContent');

catalogEntry = CatalogEntry();
		catalogEntry.set@odatatype('#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry');

		catalogEntry.setId('6b7e60db-a8e4-426a-9aed-bd12b5c0b9d4');


requestBody.setCatalogEntry($catalogEntry);

requestBody.setContent($content);

'deploymentSettings' => requestBody = DeploymentSettings();

requestBody.setDeploymentSettings($deploymentSettings);

'schedule' => requestBody = Schedule();
		requestBody.setStartDateTime('String (timestamp)');

gradualRollout = GradualRollout();
		gradualRollout.set@odatatype('#microsoft.graph.windowsUpdates.dateDrivenRolloutSettings');

		gradualRollout.setEndDateTime('String (timestamp)');


requestBody.setGradualRollout($gradualRollout);

requestBody.setSchedule($schedule);

];
requestBody.setAdditionalData(additionalData);




result = awaitclient.admin().windows().updates().updatePoliciesById('updatePolicy-id').complianceChanges().post(requestBody);


```