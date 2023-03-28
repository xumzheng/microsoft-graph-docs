---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new GetAllMessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new GetAllMessagesRequestBuilderGetQueryParameters();
$queryParameters->filter = "lastModifiedDateTime gt 2019-11-01T00:00:00Z and lastModifiedDateTime lt 2021-11-01T00:00:00Z";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->teamsById('team-id')->channels()->getAllMessages()->get($requestConfiguration);


```