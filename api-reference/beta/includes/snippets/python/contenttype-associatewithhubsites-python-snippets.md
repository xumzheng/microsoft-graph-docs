---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AssociateWithHubSitesPostRequestBody()
request_body.HubSiteUrls(['https://graph.microsoft.com/beta/sites/id', ])

request_body.propagate_to_existing_lists = False




await client.sites_by_id('site-id').contentTypes_by_id('contentType-id').associateWithHubSites.post(request_body = request_body)


```