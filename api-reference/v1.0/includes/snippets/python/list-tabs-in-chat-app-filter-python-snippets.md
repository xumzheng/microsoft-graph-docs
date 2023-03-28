---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TabsRequestBuilderGetRequestConfiguration();

$queryParameters = new TabsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["teamsApp"];
$queryParameters->filter = "teamsApp/id eq 'com.microsoft.teamspace.tab.web'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->chatsById('chat-id')->tabs()->get($requestConfiguration);


```