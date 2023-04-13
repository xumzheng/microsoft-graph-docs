---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AgreementFileLocalization()
request_body.fileName = 'Contoso ToU for guest users (French)'

request_body.language = 'fr-FR'

request_body.is_default = False

request_body.is_major_version = False

request_body.displayName = 'Contoso ToU for guest users (French)'

file_data = AgreementFileData()
FileData.Data(base64_decode('base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data'))


request_body.file_data = fileData



result = await client.identityGovernance.termsOfUse.agreements_by_id('agreement-id').files.post(request_body = request_body)


```