---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CrossCloudGovernmentOrganizationMappingPostRequestBody();

request_config = CrossCloudGovernmentOrganizationMappingRequestBuilderPostRequestConfiguration();

headers = [
	'X-MS-CloudPC-USGovCloudTenantAADToken' => '{token}',
];

request_config.headers = headers;


awaitclient.deviceManagement().virtualEndpoint().crossCloudGovernmentOrganizationMapping().post(requestBody, request_config);


```