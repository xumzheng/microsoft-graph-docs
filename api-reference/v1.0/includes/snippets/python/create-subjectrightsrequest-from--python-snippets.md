---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SubjectRightsRequest()
request_body.setType(SubjectRightsRequestType('subjectrightsrequesttype'))

request_body.setDataSubjectType(DataSubjectType('datasubjecttype'))

request_body.setRegulations(['String', ])

request_body.setDisplayName('String')

request_body.setDescription('String')

request_body.setInternalDueDateTime(DateTime('String (timestamp)'))

dataSubject = DataSubject()
dataSubject.setFirstName('String')

dataSubject.setLastName('String')

dataSubject.setEmail('String')

dataSubject.setResidency('String')

additionalData = [
'phoneNumber' => 'String', 
'SSN' => 'String', 
];
dataSubject.setAdditionalData(additionalData)



request_body.setDataSubject($dataSubject)


result = await client.privacy.subjectRightsRequests.post(request_body)


```