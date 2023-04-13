---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
on_premises_publishing = OnPremisesPublishing()
onPremisesPublishing.ExternalAuthenticationType(ExternalAuthenticationType('aadpreauthentication'))

onPremisesPublishing.internalUrl = 'https://contosoiwaapp.com'

onPremisesPublishing.externalUrl = 'https://contosoiwaapp-contoso.msappproxy.net'

onPremisesPublishing.is_http_only_cookie_enabled = True

onPremisesPublishing.is_on_prem_publishing_enabled = True

onPremisesPublishing.is_persistent_cookie_enabled = True

onPremisesPublishing.is_secure_cookie_enabled = True

onPremisesPublishing.is_state_session_enabled = True

onPremisesPublishing.is_translate_host_header_enabled = True

onPremisesPublishing.is_translate_links_in_body_enabled = True


request_body.on_premises_publishing = onPremisesPublishing



result = await client.applications_by_id('application-id').patch(request_body = request_body)


```