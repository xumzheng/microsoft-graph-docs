---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AssociateWithHubSitesPostRequestBody();
requestBody.setHubSiteUrls(['https://graph.microsoft.com/beta/sites/id', ]);

requestBody.setPropagateToExistingLists(false);



awaitclient.sitesById('site-id').contentTypesById('contentType-id').associateWithHubSites().post(requestBody);


```