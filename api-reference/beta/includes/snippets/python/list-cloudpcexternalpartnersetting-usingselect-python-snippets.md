---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ExternalPartnerSettingsRequestBuilderGetRequestConfiguration(
request_configuration = ExternalPartnerSettingsRequestBuilderGetRequestConfiguration(query_params=query_params = ExternalPartnerSettingsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","partnerId","enableConnection"]

)
query_params = ExternalPartnerSettingsRequestBuilderGetQueryParameters()
query_params['select'] = ["id","partnerId","enableConnection"]

)


result = await client.deviceManagement.virtualEndpoint.externalPartnerSettings.get(request_configuration)


```