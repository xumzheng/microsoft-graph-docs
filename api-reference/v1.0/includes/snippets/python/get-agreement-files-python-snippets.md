---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AgreementRequestBuilderGetRequestConfiguration();

$queryParameters = new AgreementRequestBuilderGetQueryParameters();
$queryParameters.expand = ["files"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().termsOfUse().agreementsById('agreement-id').get($requestConfiguration);


```