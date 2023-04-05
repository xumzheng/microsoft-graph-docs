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
		singleSignOnSettingsKerberosSignOnSettings.setKerberosServicePrincipalName('HTTP/iwademo.contoso.com')

		singleSignOnSettingsKerberosSignOnSettings.setKerberosSignOnMappingAttributeType('userPrincipalName')


singleSignOnSettings.setKerberosSignOnSettings($singleSignOnSettingsKerberosSignOnSettings)
		singleSignOnSettings.setSingleSignOnMode('onPremisesKerberos')


request_body.setSingleSignOnSettings($singleSignOnSettings)

request_body.setOnPremisesPublishing($onPremisesPublishing)

];
request_body.setAdditionalData(additionalData)




await client.applications._by_id('application-id').patch(request_body)


```