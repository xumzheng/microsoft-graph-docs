---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ChannelsRequestBuilderGetRequestConfiguration();

$queryParameters = new ChannelsRequestBuilderGetQueryParameters();
$queryParameters->filter = "membershipType eq 'private'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->teamsById('team-id')->channels()->get($requestConfiguration);


```