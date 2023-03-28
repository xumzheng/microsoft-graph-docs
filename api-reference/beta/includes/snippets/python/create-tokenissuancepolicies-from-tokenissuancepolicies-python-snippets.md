---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TokenIssuancePolicy();
$requestBody.setDefinition(['definition-value', ]);

$requestBody.setDisplayName('displayName-value');

$requestBody.setIsOrganizationDefault(true);



$requestResult = $graphServiceClient.policies().tokenIssuancePolicies().post($requestBody);


```