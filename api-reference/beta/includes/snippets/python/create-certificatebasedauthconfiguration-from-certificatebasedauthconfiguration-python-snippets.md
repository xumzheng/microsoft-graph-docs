---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CertificateBasedAuthConfigurationPostRequestBody()
additionalData = [
'certificateAuthorities' => certificateAuthorities1 = ()
		certificateAuthorities1.setIsRootAuthority(true)

		certificateAuthorities1.setCertificate('Binary')


certificateAuthoritiesArray []= certificateAuthorities1;
request_body.setCertificateAuthorities(certificateAuthoritiesArray)


];
request_body.setAdditionalData(additionalData)




await client.organizationby_id('organization-id').certificateBasedAuthConfiguration.post(request_body)


```