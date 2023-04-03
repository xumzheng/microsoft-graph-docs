---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CrossCloudGovernmentOrganizationMappingPostRequestBody();

requestConfiguration = CrossCloudGovernmentOrganizationMappingRequestBuilderPostRequestConfiguration();

headers = [
	'X-MS-CloudPC-USGovCloudTenantAADToken' => '{token}',
];

requestConfiguration.headers = headers;


graphServiceClient.deviceManagement().virtualEndpoint().crossCloudGovernmentOrganizationMapping().post(requestBody, requestConfiguration);


```