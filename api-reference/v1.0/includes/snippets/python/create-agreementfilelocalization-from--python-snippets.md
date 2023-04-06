---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AgreementFileLocalization()
request_body.setFileName('Contoso ToU for guest users (French)')

request_body.setLanguage('fr-FR')

request_body.setIsDefault(false)

request_body.setIsMajorVersion(false)

request_body.setDisplayName('Contoso ToU for guest users (French)')

fileData = AgreementFileData()
FileData.setData(base64_decode('base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data'))


request_body.setFileData($fileData)


result = await client.identityGovernance.termsOfUse.agreements_by_id('agreement-id').files.post(request_body, headers=)


```