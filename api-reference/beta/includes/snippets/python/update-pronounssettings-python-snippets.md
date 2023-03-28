---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PronounsSettings();
$requestBody.setIsEnabledInOrganization(true);



$requestResult = $graphServiceClient.organizationById('organization-id').settings().pronouns().patch($requestBody);


```