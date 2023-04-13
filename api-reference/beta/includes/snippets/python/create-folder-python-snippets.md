---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DriveItem()
request_body.name = 'New Folder'

folder = Folder()

request_body.folder = folder
additionalData = [
'@microsoft.graph.conflictBehavior' => 'rename', 
];
request_body.additionaldata(additionalData)





result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').children.post(request_body = request_body)


```