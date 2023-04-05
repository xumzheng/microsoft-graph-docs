---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AssociateWithHubSitesPostRequestBody()
request_body.setHubSiteUrls(['https://graph.microsoft.com/v1.0/sites/{site-id}', ])

request_body.setPropagateToExistingLists(false)



await client.sitesby_id('site-id')_contentTypesby_id('contentType-id')_associateWithHubSites.post(request_body)


```