---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentRequest();
request_body.setRequestType('UserAdd');

accessPackageAssignment = AccessPackageAssignment();
accessPackageAssignment.setTargetId('46184453-e63b-4f20-86c2-c557ed5d5df9');

accessPackageAssignment.setAssignmentPolicyId('2264bf65-76ba-417b-a27d-54d291f0cbc8');

accessPackageAssignment.setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b');


request_body.setAccessPackageAssignment($accessPackageAssignment);
answersAccessPackageAnswer1 = AccessPackageAnswer();
answersAccessPackageAnswer1.set@odatatype('#microsoft.graph.accessPackageAnswerString');

answersAccessPackageAnswer1AnsweredQuestion = AccessPackageQuestion();
answersAccessPackageAnswer1AnsweredQuestion.set@odatatype('#microsoft.graph.accessPackageMultipleChoiceQuestion');

answersAccessPackageAnswer1AnsweredQuestion.setId('A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF');


answersAccessPackageAnswer1.setAnsweredQuestion($answersAccessPackageAnswer1AnsweredQuestion);
additionalData = [
'value' => 'Arizona', 
];
answersAccessPackageAnswer1.setAdditionalData(additionalData);



answersArray []= answersAccessPackageAnswer1;
answersAccessPackageAnswer2 = AccessPackageAnswer();
answersAccessPackageAnswer2.set@odatatype('#microsoft.graph.accessPackageAnswerString');

answersAccessPackageAnswer2AnsweredQuestion = AccessPackageQuestion();
answersAccessPackageAnswer2AnsweredQuestion.set@odatatype('#microsoft.graph.accessPackageTextInputQuestion');

answersAccessPackageAnswer2AnsweredQuestion.setId('AA615EE9-D9D8-4C03-BE91-BEE37106DEDA');


answersAccessPackageAnswer2.setAnsweredQuestion($answersAccessPackageAnswer2AnsweredQuestion);
additionalData = [
'value' => 'Need access to marketing campaign material', 
];
answersAccessPackageAnswer2.setAdditionalData(additionalData);



answersArray []= answersAccessPackageAnswer2;
request_body.setAnswers(answersArray);




result = await client.identityGovernance().entitlementManagement().accessPackageAssignmentRequests().post(request_body);


```