---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Application()
request_body.setTags(['HR', 'Payroll', 'HideApp', ])

info = InformationalUrl()
info.setLogoUrl('https://cdn.pixabay.com/photo/2016/03/21/23/25/link-1271843_1280.png')

info.setMarketingUrl('https://www.contoso.com/app/marketing')

info.setPrivacyStatementUrl('https://www.contoso.com/app/privacy')

info.setSupportUrl('https://www.contoso.com/app/support')

info.setTermsOfServiceUrl('https://www.contoso.com/app/termsofservice')


request_body.setInfo($info)
web = WebApplication()
web.setHomePageUrl('https://www.contoso.com/')

web.setLogoutUrl('https://www.contoso.com/frontchannel_logout')

web.setRedirectUris(['https://localhost', ])


request_body.setWeb($web)
request_body.setServiceManagementReference('Owners aliases: Finance @ contosofinance@contoso.com; The Phone Company HR consulting @ hronsite@thephone-company.com;')



result = await client.applicationsById('application-id').patch(request_body)


```