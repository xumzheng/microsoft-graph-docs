---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PublishPostRequestBody();
requestBody.setRevision('1.0');



result = awaitclient.admin().edge().internetExplorerMode().siteListsById('browserSiteList-id').publish().post(requestBody);


```