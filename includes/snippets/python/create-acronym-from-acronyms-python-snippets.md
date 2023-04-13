---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Acronym()
request_body.displayName = 'GDPR'

request_body.standsFor = 'General Data Protection Regulation'

request_body.description = 'A European Union (EU) regulation on data protection and privacy in the EU and the European Economic Area (EEA) that enhances individuals\' control and rights over their personal data, simplifies the regulatory environment for international business, and addresses the transfer of personal data outside the EU and EEA areas.'

request_body.webUrl = 'http://contoso.com/GDPR'

request_body.State(AnswerState('published'))




result = await client.search.acronyms.post(request_body = request_body)


```