---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new EventRequestBuilderGetRequestConfiguration();

$queryParameters = new EventRequestBuilderGetQueryParameters();
$queryParameters.select = ["subject","body","bodyPreview","organizer","attendees","start","end","location","locations"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().eventsById('event-id').get($requestConfiguration);


```