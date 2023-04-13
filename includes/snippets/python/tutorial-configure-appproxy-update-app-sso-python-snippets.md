---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
additionalData = [
'onPremisesPublishing' => request_body = OnPremisesPublishing()
singleSignOnSettings = SingleSignOnSettings()
singleSignOnSettingsKerberosSignOnSettings = KerberosSignOnSettings()
		singleSignOnSettingsKerberosSignOnSettings.kerberosServicePrincipalName = 'HTTP/iwademo.contoso.com'

		singleSignOnSettingsKerberosSignOnSettings.kerberosSignOnMappingAttributeType = 'userPrincipalName'


singleSignOnSettings.kerberosSignOnSettings = singleSignOnSettingsKerberosSignOnSettings
		singleSignOnSettings.singleSignOnMode = 'onPremisesKerberos'


request_body.singleSignOnSettings = singleSignOnSettings

request_body.onPremisesPublishing = onPremisesPublishing

];
request_body.additionaldata(additionalData)





await client.applications_by_id('application-id').patch(request_body = request_body)


```