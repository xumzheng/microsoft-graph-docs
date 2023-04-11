---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ServicePrincipal()
customSecurityAttributes = CustomSecurityAttributeValue()
additionalData = [
'Engineering' => customSecurityAttributes = Engineering()
		customSecurityAttributes.@odatatype = '#Microsoft.DirectoryServices.CustomSecurityAttributeValue'

		customSecurityAttributes.projectDate = '2022-10-01'


customSecurityAttributes.Engineering = engineering

];
customSecurityAttributes.additionaldata(additionalData)



request_body.customSecurityAttributes = customSecurityAttributes


request_configuration = ServicePrincipalRequestBuilderPatchRequestConfiguration(
)


result = await client.servicePrincipals_by_id('servicePrincipal-id').patch(request_body = request_body)


```