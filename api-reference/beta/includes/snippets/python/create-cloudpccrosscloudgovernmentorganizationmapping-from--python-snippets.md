---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CrossCloudGovernmentOrganizationMappingPostRequestBody()

request_config = CrossCloudGovernmentOrganizationMappingRequestBuilderPostRequestConfiguration()

headers = [
	'X-MS-CloudPC-USGovCloudTenantAADToken' => '{token}',
]

request_config.headers = headers


await client.deviceManagement.virtualEndpoint.crossCloudGovernmentOrganizationMapping.post(request_body, request_config)


```