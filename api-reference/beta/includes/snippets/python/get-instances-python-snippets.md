---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new InstancesRequestBuilderGetRequestConfiguration();

$queryParameters = new InstancesRequestBuilderGetQueryParameters();
$queryParameters.startDateTime = "2019-04-08T09:00:00.0000000";
$queryParameters.endDateTime = "2019-04-30T09:00:00.0000000";
$queryParameters.select = ["subject","bodyPreview","seriesMasterId","type","recurrence","start","end"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().eventsById('event-id').instances().get($requestConfiguration);


```