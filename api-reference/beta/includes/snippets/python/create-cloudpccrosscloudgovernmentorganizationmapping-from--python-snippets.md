---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CrossCloudGovernmentOrganizationMappingPostRequestBody()

request_config = CrossCloudGovernmentOrganizationMappingRequestBuilderPostRequestConfiguration(
request_config = CrossCloudGovernmentOrganizationMappingRequestBuilderPostRequestConfiguration(query_params=)
headers['X-MS-CloudPC-USGovCloudTenantAADToken'] = "{token}"


await client.deviceManagement.virtualEndpoint.crossCloudGovernmentOrganizationMapping.post(request_body, request_config, headers=request_config)


```