---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DocumentSetVersion();
requestBody.setComment('v1');

requestBody.setShouldCaptureMinorVersion(false);



result = await client.sitesById('site-id').listsById('list-id').itemsById('listItem-id').documentSetVersions().post(requestBody);


```