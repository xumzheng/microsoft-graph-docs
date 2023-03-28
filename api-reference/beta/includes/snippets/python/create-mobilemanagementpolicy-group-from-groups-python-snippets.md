---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceCreate();
$requestBody->set@odataid('https://graph.microsoft.com/odata/groups(\'1a9db3ab-0acf-4808-99ae-e8ed581cb2e0\')');



$graphServiceClient->policies()->mobileAppManagementPoliciesById('mobilityManagementPolicy-id')->includedGroups()->ref()->post($requestBody);


```