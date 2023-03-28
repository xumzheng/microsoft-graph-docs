---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new GroupsRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupsRequestBuilderGetQueryParameters();
$queryParameters.filter = "mailEnabled eq false and securityEnabled eq true and NOT) and membershipRuleProcessingState eq 'On'";
$queryParameters.count = true;
$queryParameters.select = ["id","membershipRule","membershipRuleProcessingState"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.groups().get($requestConfiguration);


```