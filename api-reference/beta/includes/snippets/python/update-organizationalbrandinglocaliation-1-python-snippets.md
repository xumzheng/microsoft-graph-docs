---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OrganizationalBranding();
requestBody.setSignInPageText('Default');

requestBody.setUsernameHintText('DefaultHint');


requestConfiguration = BrandingRequestBuilderPatchRequestConfiguration();

headers = [
	'Accept-Language' => '0',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.organizationById('organization-id').branding().patch(requestBody, requestConfiguration);


```