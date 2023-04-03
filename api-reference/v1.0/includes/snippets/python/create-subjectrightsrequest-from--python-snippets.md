---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SubjectRightsRequest();
requestBody.setType(SubjectRightsRequestType('subjectrightsrequesttype'));

requestBody.setDataSubjectType(DataSubjectType('datasubjecttype'));

requestBody.setRegulations(['String', ]);

requestBody.setDisplayName('String');

requestBody.setDescription('String');

requestBody.setInternalDueDateTime(DateTime('String (timestamp)'));

dataSubject = DataSubject();
dataSubject.setFirstName('String');

dataSubject.setLastName('String');

dataSubject.setEmail('String');

dataSubject.setResidency('String');

additionalData = [
'phoneNumber' => 'String', 
'SSN' => 'String', 
];
dataSubject.setAdditionalData(additionalData);



requestBody.setDataSubject($dataSubject);


result = await client.privacy().subjectRightsRequests().post(requestBody);


```