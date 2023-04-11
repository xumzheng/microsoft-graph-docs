---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = CloudPcUserSettingRequestBuilder.CloudPcUserSettingRequestBuilderGetQueryParameters(
		expand = ["assignments"],
)

request_configuration = CloudPcUserSettingRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.deviceManagement.virtualEndpoint.userSettings_by_id('cloudPcUserSetting-id').get(request_configuration = request_configuration)


```