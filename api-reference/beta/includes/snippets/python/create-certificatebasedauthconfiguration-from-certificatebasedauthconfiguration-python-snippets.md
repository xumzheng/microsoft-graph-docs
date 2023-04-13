---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CertificateBasedAuthConfigurationPostRequestBody()
additionalData = [
'certificateAuthorities' => certificate_authorities1 = ()
		certificateAuthorities1.is_root_authority = True

		certificateAuthorities1.certificate = 'Binary'


certificateAuthoritiesArray []= certificateAuthorities1;
request_body.certificateauthorities(certificateAuthoritiesArray)


];
request_body.additionaldata(additionalData)





await client.organization_by_id('organization-id').certificateBasedAuthConfiguration.post(request_body = request_body)


```