---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TeamsTabRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsTabRequestBuilderGetQueryParameters();
$queryParameters->expand = ["teamsApp"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->chatsById('chat-id')->tabsById('teamsTab-id')->get($requestConfiguration);


```