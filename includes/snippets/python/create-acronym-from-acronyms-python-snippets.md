---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Acronym();
requestBody.setDisplayName('GDPR');

requestBody.setStandsFor('General Data Protection Regulation');

requestBody.setDescription('A European Union (EU) regulation on data protection and privacy in the EU and the European Economic Area (EEA) that enhances individuals\' control and rights over their personal data, simplifies the regulatory environment for international business, and addresses the transfer of personal data outside the EU and EEA areas.');

requestBody.setWebUrl('http://contoso.com/GDPR');

requestBody.setState(AnswerState('published'));



result = await client.search().acronyms().post(requestBody);


```