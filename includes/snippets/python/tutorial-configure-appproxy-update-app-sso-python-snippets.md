---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Application();
additionalData = [
'onPremisesPublishing' => requestBody = OnPremisesPublishing();
singleSignOnSettings = SingleSignOnSettings();
singleSignOnSettingsKerberosSignOnSettings = KerberosSignOnSettings();
		singleSignOnSettingsKerberosSignOnSettings.setKerberosServicePrincipalName('HTTP/iwademo.contoso.com');

		singleSignOnSettingsKerberosSignOnSettings.setKerberosSignOnMappingAttributeType('userPrincipalName');


singleSignOnSettings.setKerberosSignOnSettings($singleSignOnSettingsKerberosSignOnSettings);
		singleSignOnSettings.setSingleSignOnMode('onPremisesKerberos');


requestBody.setSingleSignOnSettings($singleSignOnSettings);

requestBody.setOnPremisesPublishing($onPremisesPublishing);

];
requestBody.setAdditionalData(additionalData);




graphServiceClient.applicationsById('application-id').patch(requestBody);


```