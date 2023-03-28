---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new DocumentSetVersion();
$requestBody.setComment('v1');

$requestBody.setShouldCaptureMinorVersion(false);



$requestResult = $graphServiceClient.sitesById('site-id').listsById('list-id').itemsById('listItem-id').documentSetVersions().post($requestBody);


```