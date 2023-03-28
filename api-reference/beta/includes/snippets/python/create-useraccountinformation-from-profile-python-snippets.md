---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UserAccountInformation();
$requestBody.setAllowedAudiences(new AllowedAudiences('organization'));

$requestBody.setCountryCode('NO');



$requestResult = $graphServiceClient.me().profile().account().post($requestBody);


```