---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = CloudPcUserSettingRequestBuilderGetRequestConfiguration(
request_configuration = CloudPcUserSettingRequestBuilderGetRequestConfiguration(query_params=query_params = CloudPcUserSettingRequestBuilderGetQueryParameters()
query_params['expand'] = ["assignments"]

)
query_params = CloudPcUserSettingRequestBuilderGetQueryParameters()
query_params['expand'] = ["assignments"]

)


result = await client.deviceManagement.virtualEndpoint.userSettings_by_id('cloudPcUserSetting-id').get(request_configuration)


```