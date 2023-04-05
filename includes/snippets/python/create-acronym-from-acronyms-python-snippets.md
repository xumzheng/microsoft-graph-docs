---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Acronym()
request_body.setDisplayName('GDPR')

request_body.setStandsFor('General Data Protection Regulation')

request_body.setDescription('A European Union (EU) regulation on data protection and privacy in the EU and the European Economic Area (EEA) that enhances individuals\' control and rights over their personal data, simplifies the regulatory environment for international business, and addresses the transfer of personal data outside the EU and EEA areas.')

request_body.setWebUrl('http://contoso.com/GDPR')

request_body.setState(AnswerState('published'))



result = await client.search_acronyms.post(request_body)


```