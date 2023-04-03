---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DeltaRequestBuilderGetRequestConfiguration();

headers = [
	'Prefer' => 'odata.maxpagesize=2',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().mailFoldersById('mailFolder-id').messages().delta().get(requestConfiguration);


```