---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PartnersRequestBuilderGetRequestConfiguration();

$queryParameters = new PartnersRequestBuilderGetQueryParameters();
$queryParameters->select = ["tenantId"];
$queryParameters->expand = ["identitySynchronization"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->policies()->crossTenantAccessPolicy()->partners()->get($requestConfiguration);


```