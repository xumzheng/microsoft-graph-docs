---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GovernanceRoleSetting();
adminEligibleSettingsGovernanceRuleSetting1 = GovernanceRuleSetting();
adminEligibleSettingsGovernanceRuleSetting1.setRuleIdentifier('ExpirationRule');

adminEligibleSettingsGovernanceRuleSetting1.setSetting('{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}');


adminEligibleSettingsArray []= adminEligibleSettingsGovernanceRuleSetting1;
requestBody.setAdminEligibleSettings(adminEligibleSettingsArray);




result = awaitclient.privilegedAccessById('privilegedAccess-id').roleSettingsById('governanceRoleSetting-id').patch(requestBody);


```