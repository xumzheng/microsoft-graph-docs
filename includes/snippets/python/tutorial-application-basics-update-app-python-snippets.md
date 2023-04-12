---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
request_body.Tags(['HR', 'Payroll', 'HideApp', ])

info = InformationalUrl()
info.logoUrl = 'https://cdn.pixabay.com/photo/2016/03/21/23/25/link-1271843_1280.png'

info.marketingUrl = 'https://www.contoso.com/app/marketing'

info.privacyStatementUrl = 'https://www.contoso.com/app/privacy'

info.supportUrl = 'https://www.contoso.com/app/support'

info.termsOfServiceUrl = 'https://www.contoso.com/app/termsofservice'


request_body.info = info
web = WebApplication()
web.homePageUrl = 'https://www.contoso.com/'

web.logoutUrl = 'https://www.contoso.com/frontchannel_logout'

web.RedirectUris(['https://localhost', ])


request_body.web = web
request_body.serviceManagementReference = 'Owners aliases: Finance @ contosofinance@contoso.com; The Phone Company HR consulting @ hronsite@thephone-company.com;'




result = await client.applications_by_id('application-id').patch(request_body = request_body)


```