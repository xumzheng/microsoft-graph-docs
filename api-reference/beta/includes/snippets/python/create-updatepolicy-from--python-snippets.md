---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UpdatePolicy();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.updatePolicy');

audience = DeploymentAudience();
audience.setId('8c4eb1eb-d7a3-4633-8e2f-f926e82df08e');


requestBody.setAudience($audience);
complianceChangesComplianceChange1 = ComplianceChange();
complianceChangesComplianceChange1.set@odatatype('#microsoft.graph.windowsUpdates.contentApproval');


complianceChangesArray []= complianceChangesComplianceChange1;
requestBody.setComplianceChanges(complianceChangesArray);


complianceChangeRulesComplianceChangeRule1 = ComplianceChangeRule();
complianceChangeRulesComplianceChangeRule1.set@odatatype('#microsoft.graph.windowsUpdates.contentApprovalRule');

additionalData = [
'contentFilter' => complianceChangeRulesComplianceChangeRule1 = ContentFilter();
	complianceChangeRulesComplianceChangeRule1.set@odatatype('#microsoft.graph.windowsUpdates.driverUpdateFilter');


complianceChangeRulesComplianceChangeRule1.setContentFilter($contentFilter);

'durationBeforeDeploymentStart' => 'P7D', 
];
complianceChangeRulesComplianceChangeRule1.setAdditionalData(additionalData);



complianceChangeRulesArray []= complianceChangeRulesComplianceChangeRule1;
requestBody.setComplianceChangeRules(complianceChangeRulesArray);


deploymentSettings = DeploymentSettings();
deploymentSettings.set@odatatype('microsoft.graph.windowsUpdates.deploymentSettings');

deploymentSettingsSchedule = ScheduleSettings();
deploymentSettingsScheduleGradualRollout = GradualRolloutSettings();
deploymentSettingsScheduleGradualRollout.set@odatatype('#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings');

$deploymentSettingsScheduleGradualRollout.setDurationBetweenOffers( \DateInterval('P1D'));

additionalData = [
'devicePerOffer' => 1000,
];
deploymentSettingsScheduleGradualRollout.setAdditionalData(additionalData);



deploymentSettingsSchedule.setGradualRollout($deploymentSettingsScheduleGradualRollout);

deploymentSettings.setSchedule($deploymentSettingsSchedule);

requestBody.setDeploymentSettings($deploymentSettings);


requestResult = graphServiceClient.admin().windows().updates().updatePolicies().post(requestBody);


```