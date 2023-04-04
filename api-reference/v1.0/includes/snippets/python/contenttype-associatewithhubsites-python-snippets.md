---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AssociateWithHubSitesPostRequestBody()
request_body.setHubSiteUrls(['https://graph.microsoft.com/v1.0/sites/{site-id}', ])

request_body.setPropagateToExistingLists(false)



await client.sitesById('site-id').contentTypesById('contentType-id').associateWithHubSites.post(request_body)


```