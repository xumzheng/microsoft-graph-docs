---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GovernanceRoleSetting();
$adminEligibleSettingsGovernanceRuleSetting1 = new GovernanceRuleSetting();
$adminEligibleSettingsGovernanceRuleSetting1.setRuleIdentifier('ExpirationRule');

$adminEligibleSettingsGovernanceRuleSetting1.setSetting('{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}');


$adminEligibleSettingsArray []= $adminEligibleSettingsGovernanceRuleSetting1;
$requestBody.setAdminEligibleSettings($adminEligibleSettingsArray);




$requestResult = $graphServiceClient.privilegedAccessById('privilegedAccess-id').roleSettingsById('governanceRoleSetting-id').patch($requestBody);


```