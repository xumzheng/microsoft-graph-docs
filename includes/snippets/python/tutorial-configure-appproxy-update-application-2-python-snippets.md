---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
onPremisesPublishing = OnPremisesPublishing()
onPremisesPublishing.ExternalAuthenticationType(ExternalAuthenticationType('aadpreauthentication'))

onPremisesPublishing.internalUrl = 'https://contosoiwaapp.com'

onPremisesPublishing.externalUrl = 'https://contosoiwaapp-contoso.msappproxy.net'

onPremisesPublishing.isHttpOnlyCookieEnabled = true

onPremisesPublishing.isOnPremPublishingEnabled = true

onPremisesPublishing.isPersistentCookieEnabled = true

onPremisesPublishing.isSecureCookieEnabled = true

onPremisesPublishing.isStateSessionEnabled = true

onPremisesPublishing.isTranslateHostHeaderEnabled = true

onPremisesPublishing.isTranslateLinksInBodyEnabled = true


request_body.onPremisesPublishing = onPremisesPublishing


request_configuration = ApplicationRequestBuilderPatchRequestConfiguration(
)


result = await client.applications_by_id('application-id').patch(request_body = request_body)


```