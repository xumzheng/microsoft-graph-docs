---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new EventsRequestBuilderGetRequestConfiguration();

$queryParameters = new EventsRequestBuilderGetQueryParameters();
$queryParameters.select = ["subject","body","bodyPreview","organizer","attendees","start","end","location"];

$headers = [
'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

$requestConfiguration.queryParameters = $queryParameters;
$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.me().events().get($requestConfiguration);


```