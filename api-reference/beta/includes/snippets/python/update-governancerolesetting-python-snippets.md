---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GovernanceRoleSetting()
adminEligibleSettingsGovernanceRuleSetting1 = GovernanceRuleSetting()
adminEligibleSettingsGovernanceRuleSetting1.setRuleIdentifier('ExpirationRule')

adminEligibleSettingsGovernanceRuleSetting1.setSetting('{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}')


adminEligibleSettingsArray []= adminEligibleSettingsGovernanceRuleSetting1;
request_body.setAdminEligibleSettings(adminEligibleSettingsArray)




result = await client.privilegedAccessById('privilegedAccess-id').roleSettingsById('governanceRoleSetting-id').patch(request_body)


```