---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Governance_role_setting()
admin_eligible_settings_governance_rule_setting1 = Governance_rule_setting()
admin_eligible_settings_governance_rule_setting1.rule_identifier = 'ExpirationRule'

admin_eligible_settings_governance_rule_setting1.setting = '{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}'


adminEligibleSettingsArray []= adminEligibleSettingsGovernanceRuleSetting1;
request_body.admineligiblesettings(adminEligibleSettingsArray)





result = await client.privileged_access.by_privileged_acce_id('privilegedAccess-id').role_settings.by_role_setting_id('governanceRoleSetting-id').patch(request_body = request_body)


```