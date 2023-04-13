---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PublishPostRequestBody()
request_body.revision = '1.0'

sitesBrowserSite1 = BrowserSite()
sitesBrowserSite1.id = '53e5f971-fc7b-4cd3-a1bf-34d7c0416882'


sitesArray []= sitesBrowserSite1;
sitesBrowserSite2 = BrowserSite()
sitesBrowserSite2.id = '2e27cc86-3662-447e-b751-274fb9f869ea'


sitesArray []= sitesBrowserSite2;
request_body.sites(sitesArray)


sharedCookiesBrowserSharedCookie1 = BrowserSharedCookie()
sharedCookiesBrowserSharedCookie1.id = '7f639835-23ab-4793-b1e6-1a06fad127a2'


sharedCookiesArray []= sharedCookiesBrowserSharedCookie1;
request_body.sharedcookies(sharedCookiesArray)





result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').publish.post(request_body = request_body)


```