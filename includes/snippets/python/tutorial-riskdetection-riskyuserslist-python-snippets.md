---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new RiskyUsersRequestBuilderGetRequestConfiguration();

$queryParameters = new RiskyUsersRequestBuilderGetQueryParameters();
$queryParameters->filter = "userDisplayName eq 'MyTestUser1'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identityProtection()->riskyUsers()->get($requestConfiguration);


```