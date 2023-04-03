---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AgreementFileLocalization();
requestBody.setFileName('Contoso ToU for guest users (French)');

requestBody.setLanguage('fr-FR');

requestBody.setIsDefault(false);

requestBody.setIsMajorVersion(false);

requestBody.setDisplayName('Contoso ToU for guest users (French)');

fileData = AgreementFileData();
FileData.setData(base64_decode('base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data'));


requestBody.setFileData($fileData);


requestResult = graphServiceClient.identityGovernance().termsOfUse().agreementsById('agreement-id').files().post(requestBody);


```