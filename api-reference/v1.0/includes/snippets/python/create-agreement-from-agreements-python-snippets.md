---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Agreement()
request_body.displayName = 'Contoso ToU for guest users'

request_body.is_viewing_before_acceptance_required = True

files_agreement_file_localization1 = AgreementFileLocalization()
filesAgreementFileLocalization1.fileName = 'TOU.pdf'

filesAgreementFileLocalization1.language = 'en'

filesAgreementFileLocalization1.is_default = True

files_agreement_file_localization1_file_data = AgreementFileData()
filesAgreementFileLocalization1FileData.Data(base64_decode('SGVsbG8gd29ybGQ=//truncated-binary'))


filesAgreementFileLocalization1.file_data = filesAgreementFileLocalization1FileData

filesArray []= filesAgreementFileLocalization1;
request_body.files(filesArray)





result = await client.identityGovernance.termsOfUse.agreements.post(request_body = request_body)


```