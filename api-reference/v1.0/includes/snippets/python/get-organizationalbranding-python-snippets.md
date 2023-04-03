---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = BrandingRequestBuilderGetRequestConfiguration();

headers = [
	'Accept-Language' => '0',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.organizationById('organization-id').branding().get(requestConfiguration);


```