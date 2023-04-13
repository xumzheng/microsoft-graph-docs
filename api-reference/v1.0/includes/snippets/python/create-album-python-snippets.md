---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DriveItem()
request_body.name = 'My Day at the Beach'

bundle = Bundle()
bundle_album = Album()

bundle.album = bundleAlbum

request_body.bundle = bundle
children_drive_item1 = DriveItem()
childrenDriveItem1.id = '1234asdf'


childrenArray []= childrenDriveItem1;
request_body.children(childrenArray)


additionalData = [
'@microsoft.graph.conflictBehavior' => 'rename', 
];
request_body.additionaldata(additionalData)





result = await client.drives_by_id('drive-id').bundles.post(request_body = request_body)


```