---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Application()
keyCredentialsKeyCredential1 = KeyCredential()
keyCredentialsKeyCredential1.endDateTime = DateTime('2024-01-11T15:31:26Z')

keyCredentialsKeyCredential1.startDateTime = DateTime('2023-01-12T15:31:26Z')

keyCredentialsKeyCredential1.type = 'AsymmetricX509Cert'

keyCredentialsKeyCredential1.usage = 'Verify'

keyCredentialsKeyCredential1.Key(base64_decode('base64MIIDADCCAeigAwIBAgIQP6HEGDdZ65xJTcK4dCBvZzANBgkqhkiG9w0BAQsFADATMREwDwYDVQQDDAgyMDIzMDExMjAeFw0yMzAxMTIwODExNTZaFw0yNDAxMTIwODMxNTZaMBMxETAPBgNVBAMMCDIwMjMwMTEyMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAseKf1weEacJ67D6/...laxQPUbuIL+DaXVkKRm1V3GgIpKTBqMzTf4tCpy7rpUZbhcwAFw6h9A=='))

keyCredentialsKeyCredential1.displayName = 'CN=20230112'


keyCredentialsArray []= keyCredentialsKeyCredential1;
request_body.keycredentials(keyCredentialsArray)





result = await client.applications_by_id('application-id').patch(request_body = request_body)


```