---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Agreement();
requestBody.setDisplayName('Contoso ToU for guest users');

requestBody.setIsViewingBeforeAcceptanceRequired(true);

filesAgreementFileLocalization1 = AgreementFileLocalization();
filesAgreementFileLocalization1.setFileName('TOU.pdf');

filesAgreementFileLocalization1.setLanguage('en');

filesAgreementFileLocalization1.setIsDefault(true);

filesAgreementFileLocalization1FileData = AgreementFileData();
filesAgreementFileLocalization1FileData.setData(base64_decode('SGVsbG8gd29ybGQ=//truncated-binary'));


filesAgreementFileLocalization1.setFileData($filesAgreementFileLocalization1FileData);

filesArray []= filesAgreementFileLocalization1;
requestBody.setFiles(filesArray);




result = awaitclient.identityGovernance().termsOfUse().agreements().post(requestBody);


```