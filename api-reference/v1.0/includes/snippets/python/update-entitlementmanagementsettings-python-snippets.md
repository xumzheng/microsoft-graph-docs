---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EntitlementManagementSettings();
$requestBody.setExternalUserLifecycleAction(new AccessPackageExternalUserLifecycleAction('none'));



$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().settings().patch($requestBody);


```