---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DocumentSetVersion()
request_body.setComment('v1')

request_body.setShouldCaptureMinorVersion(false)



result = await client.sitesById('site-id').listsById('list-id').itemsById('listItem-id').documentSetVersions.post(request_body)


```