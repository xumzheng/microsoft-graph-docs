---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new InsightsSettings();
$requestBody.setIsEnabledInOrganization(true);

$requestBody.setDisabledForGroup('edbfe4fb-ec70-4300-928f-dbb2ae86c981');



$requestResult = $graphServiceClient.organizationById('organization-id').settings().contactInsights().patch($requestBody);


```