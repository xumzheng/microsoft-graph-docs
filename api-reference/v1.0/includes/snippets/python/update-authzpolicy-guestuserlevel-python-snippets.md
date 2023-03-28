---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthorizationPolicy();
$requestBody.setAllowEmailVerifiedUsersToJoinOrganization(false);



$requestResult = $graphServiceClient.policies().authorizationPolicy().patch($requestBody);


```