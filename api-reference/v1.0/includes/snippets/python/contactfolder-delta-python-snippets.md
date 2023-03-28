---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$headers = [
	'Prefer' => 'odata.maxpagesize=2',
];

$requestConfiguration->headers = $headers;


$requestResult = $graphServiceClient->me()->contactFolders()->delta()->get($requestConfiguration);


```