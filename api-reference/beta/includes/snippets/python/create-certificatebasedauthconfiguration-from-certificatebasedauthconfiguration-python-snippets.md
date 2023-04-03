---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CertificateBasedAuthConfigurationPostRequestBody();
additionalData = [
'certificateAuthorities' => certificateAuthorities1 = ();
		certificateAuthorities1.setIsRootAuthority(true);

		certificateAuthorities1.setCertificate('Binary');


certificateAuthoritiesArray []= certificateAuthorities1;
requestBody.setCertificateAuthorities(certificateAuthoritiesArray);


];
requestBody.setAdditionalData(additionalData);




graphServiceClient.organizationById('organization-id').certificateBasedAuthConfiguration().post(requestBody);


```