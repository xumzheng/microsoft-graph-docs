---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
additionalData = [
'onPremisesPublishing' => request_body = OnPremisesPublishing()
single_sign_on_settings = SingleSignOnSettings()
single_sign_on_settings_kerberos_sign_on_settings = KerberosSignOnSettings()
		singleSignOnSettingsKerberosSignOnSettings.kerberosServicePrincipalName = 'HTTP/iwademo.contoso.com'

		singleSignOnSettingsKerberosSignOnSettings.kerberosSignOnMappingAttributeType = 'userPrincipalName'


singleSignOnSettings.kerberos_sign_on_settings = singleSignOnSettingsKerberosSignOnSettings
		singleSignOnSettings.singleSignOnMode = 'onPremisesKerberos'


request_body.single_sign_on_settings = singleSignOnSettings

request_body.on_premises_publishing = onPremisesPublishing

];
request_body.additionaldata(additionalData)





await client.applications_by_id('application-id').patch(request_body = request_body)


```