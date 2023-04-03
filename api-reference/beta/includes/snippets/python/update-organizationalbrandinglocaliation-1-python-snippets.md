---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OrganizationalBranding();
requestBody.setSignInPageText('Default');

requestBody.setUsernameHintText('DefaultHint');


request_config = BrandingRequestBuilderPatchRequestConfiguration();

headers = [
	'Accept-Language' => '0',
];

request_config.headers = headers;


result = awaitclient.organizationById('organization-id').branding().patch(requestBody, request_config);


```