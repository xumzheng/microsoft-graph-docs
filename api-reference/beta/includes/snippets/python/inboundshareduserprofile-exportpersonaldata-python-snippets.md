---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPersonalDataPostRequestBody()
request_body.setStorageLocation('MyStorageAccount')


request_config = ExportPersonalDataRequestBuilderPostRequestConfiguration(
request_config = ExportPersonalDataRequestBuilderPostRequestConfiguration(query_params=)


await client.directory.inboundSharedUserProfiles_by_id('inboundSharedUserProfile-userId').exportPersonalData.post(request_body, headers=)


```