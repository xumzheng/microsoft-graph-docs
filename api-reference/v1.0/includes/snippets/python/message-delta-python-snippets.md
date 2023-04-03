---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = DeltaRequestBuilderGetRequestConfiguration();

headers = [
	'Prefer' => 'odata.maxpagesize=2',
];

request_config.headers = headers;


result = awaitclient.me().mailFoldersById('mailFolder-id').messages().delta().get(request_config);


```