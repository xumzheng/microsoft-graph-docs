---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CloudPcProvisioningPolicy();
requestBody.set@odatatype('#microsoft.graph.cloudPcProvisioningPolicy');

requestBody.setDisplayName('HR provisioning policy');

requestBody.setDescription('Provisioning policy for India HR employees');

requestBody.setOnPremisesConnectionId('4e47d0f6-6f77-44f0-8893-c0fe1701ffff');

requestBody.setImageId('Image ID value');

requestBody.setImageDisplayName('Image Display Name value');

requestBody.setImageType(CloudPcProvisioningPolicyImageType('custom'));

windowsSettings = CloudPcWindowsSettings();
windowsSettings.setLanguage('en-US');


requestBody.setWindowsSettings($windowsSettings);


requestResult = graphServiceClient.deviceManagement().virtualEndpoint().provisioningPoliciesById('cloudPcProvisioningPolicy-id').patch(requestBody);


```