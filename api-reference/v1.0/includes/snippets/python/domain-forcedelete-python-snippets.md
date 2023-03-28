---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ForceDeletePostRequestBody();
$requestBody->setDisableUserAccounts(true);



$graphServiceClient->domainsById('domain-id')->forceDelete()->post($requestBody);


```