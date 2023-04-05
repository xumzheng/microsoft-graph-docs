---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ComplianceChange()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.contentApproval')

additionalData = [
'content' => request_body = Content()
		request_body.set@odatatype('#microsoft.graph.windowsUpdates.catalogContent')

catalogEntry = CatalogEntry()
		catalogEntry.set@odatatype('#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')

		catalogEntry.setId('6b7e60db-a8e4-426a-9aed-bd12b5c0b9d4')


request_body.setCatalogEntry($catalogEntry)

request_body.setContent($content)

'deploymentSettings' => request_body = DeploymentSettings()

request_body.setDeploymentSettings($deploymentSettings)

'schedule' => request_body = Schedule()
		request_body.setStartDateTime('String (timestamp)')

gradualRollout = GradualRollout()
		gradualRollout.set@odatatype('#microsoft.graph.windowsUpdates.dateDrivenRolloutSettings')

		gradualRollout.setEndDateTime('String (timestamp)')


request_body.setGradualRollout($gradualRollout)

request_body.setSchedule($schedule)

];
request_body.setAdditionalData(additionalData)




result = await client.admin.windows.updates.updatePoliciesById('updatePolicy-id').complianceChanges.post(request_body)


```