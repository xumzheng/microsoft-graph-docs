---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CertificateBasedAuthConfigurationPostRequestBody();
additionalData = [
'certificateAuthorities' => certificateAuthorities1 = ();
		certificateAuthorities1.setIsRootAuthority(true);

		certificateAuthorities1.setCertificate('Binary');


certificateAuthoritiesArray []= certificateAuthorities1;
requestBody.setCertificateAuthorities(certificateAuthoritiesArray);


];
requestBody.setAdditionalData(additionalData);




awaitclient.organizationById('organization-id').certificateBasedAuthConfiguration().post(requestBody);


```