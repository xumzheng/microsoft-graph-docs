---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GovernanceRoleSetting()
admin_eligible_settings_governance_rule_setting1 = GovernanceRuleSetting()
adminEligibleSettingsGovernanceRuleSetting1.ruleIdentifier = 'ExpirationRule'

adminEligibleSettingsGovernanceRuleSetting1.setting = '{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}'


adminEligibleSettingsArray []= adminEligibleSettingsGovernanceRuleSetting1;
request_body.admineligiblesettings(adminEligibleSettingsArray)





result = await client.privilegedAccess_by_id('privilegedAccess-id').roleSettings_by_id('governanceRoleSetting-id').patch(request_body = request_body)


```