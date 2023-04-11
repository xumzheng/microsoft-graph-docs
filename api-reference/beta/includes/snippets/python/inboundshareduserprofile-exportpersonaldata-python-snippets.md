---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPersonalDataPostRequestBody()
request_body.storageLocation = 'MyStorageAccount'



request_configuration = ExportPersonalDataRequestBuilderPostRequestConfiguration(
)


await client.directory.inboundSharedUserProfiles_by_id('inboundSharedUserProfile-userId').exportPersonalData.post(request_body = request_body)


```