---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new OutlookTaskRequestBuilderGetRequestConfiguration();

$headers = [
	'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.me().outlook().tasksById('outlookTask-id').get($requestConfiguration);


```