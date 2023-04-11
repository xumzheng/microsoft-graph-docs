---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdatePolicy()
request_body.@odatatype = '#microsoft.graph.windowsUpdates.updatePolicy'

audience = DeploymentAudience()
audience.id = '8c4eb1eb-d7a3-4633-8e2f-f926e82df08e'


request_body.audience = audience
complianceChangesComplianceChange1 = ComplianceChange()
complianceChangesComplianceChange1.@odatatype = '#microsoft.graph.windowsUpdates.contentApproval'


complianceChangesArray []= complianceChangesComplianceChange1;
request_body.compliancechanges(complianceChangesArray)


complianceChangeRulesComplianceChangeRule1 = ComplianceChangeRule()
complianceChangeRulesComplianceChangeRule1.@odatatype = '#microsoft.graph.windowsUpdates.contentApprovalRule'

additionalData = [
'contentFilter' => complianceChangeRulesComplianceChangeRule1 = ContentFilter()
	complianceChangeRulesComplianceChangeRule1.@odatatype = '#microsoft.graph.windowsUpdates.driverUpdateFilter'


complianceChangeRulesComplianceChangeRule1.contentFilter = contentFilter

'durationBeforeDeploymentStart' => 'P7D', 
];
complianceChangeRulesComplianceChangeRule1.additionaldata(additionalData)



complianceChangeRulesArray []= complianceChangeRulesComplianceChangeRule1;
request_body.compliancechangerules(complianceChangeRulesArray)


deploymentSettings = DeploymentSettings()
deploymentSettings.@odatatype = 'microsoft.graph.windowsUpdates.deploymentSettings'

deploymentSettingsSchedule = ScheduleSettings()
deploymentSettingsScheduleGradualRollout = GradualRolloutSettings()
deploymentSettingsScheduleGradualRollout.@odatatype = '#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings'

deploymentSettingsScheduleGradualRollout.durationbetweenoffers =  \DateInterval('P1D')

additionalData = [
'devicePerOffer' => 1000,
];
deploymentSettingsScheduleGradualRollout.additionaldata(additionalData)



deploymentSettingsSchedule.gradualRollout = deploymentSettingsScheduleGradualRollout

deploymentSettings.schedule = deploymentSettingsSchedule

request_body.deploymentSettings = deploymentSettings


request_configuration = UpdatePoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.admin.windows.updates.updatePolicies.post(request_body = request_body)


```