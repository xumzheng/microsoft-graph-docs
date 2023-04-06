---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
onPremisesPublishing = OnPremisesPublishing()
onPremisesPublishing.setExternalAuthenticationType(ExternalAuthenticationType('aadpreauthentication'))

onPremisesPublishing.setInternalUrl('https://contosoiwaapp.com')

onPremisesPublishing.setExternalUrl('https://contosoiwaapp-contoso.msappproxy.net')

onPremisesPublishing.setIsHttpOnlyCookieEnabled(true)

onPremisesPublishing.setIsOnPremPublishingEnabled(true)

onPremisesPublishing.setIsPersistentCookieEnabled(true)

onPremisesPublishing.setIsSecureCookieEnabled(true)

onPremisesPublishing.setIsStateSessionEnabled(true)

onPremisesPublishing.setIsTranslateHostHeaderEnabled(true)

onPremisesPublishing.setIsTranslateLinksInBodyEnabled(true)


request_body.setOnPremisesPublishing($onPremisesPublishing)


result = await client.applications_by_id('application-id').patch(request_body, headers=)


```