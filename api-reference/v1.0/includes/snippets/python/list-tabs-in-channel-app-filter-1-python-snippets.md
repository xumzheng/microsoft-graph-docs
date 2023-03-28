---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TabsRequestBuilderGetRequestConfiguration();

$queryParameters = new TabsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["teamsApp"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->teamsById('team-id')->channelsById('channel-id')->tabs()->get($requestConfiguration);


```