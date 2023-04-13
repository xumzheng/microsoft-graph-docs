---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ComplianceChange()
request_body.@odatatype = '#microsoft.graph.windowsUpdates.contentApproval'

additionalData = [
'content' => request_body = Content()
		request_body.@odatatype = '#microsoft.graph.windowsUpdates.catalogContent'

catalog_entry = CatalogEntry()
		catalogEntry.@odatatype = '#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry'

		catalogEntry.id = '6b7e60db-a8e4-426a-9aed-bd12b5c0b9d4'


request_body.catalog_entry = catalogEntry

request_body.content = content

'deploymentSettings' => request_body = DeploymentSettings()

request_body.deployment_settings = deploymentSettings

'schedule' => request_body = Schedule()
		request_body.startDateTime = 'String (timestamp)'

gradual_rollout = GradualRollout()
		gradualRollout.@odatatype = '#microsoft.graph.windowsUpdates.dateDrivenRolloutSettings'

		gradualRollout.endDateTime = 'String (timestamp)'


request_body.gradual_rollout = gradualRollout

request_body.schedule = schedule

];
request_body.additionaldata(additionalData)





result = await client.admin.windows.updates.updatePolicies_by_id('updatePolicy-id').complianceChanges.post(request_body = request_body)


```