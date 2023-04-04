---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentRequest();
request_body.set@odatatype('#microsoft.graph.accessPackageAssignmentRequest');

request_body.setRequestType(AccessPackageRequestType('useradd'));

answersAccessPackageAnswer1 = AccessPackageAnswer();
answersAccessPackageAnswer1.set@odatatype('#microsoft.graph.accessPackageAnswerString');

answersAccessPackageAnswer1.setDisplayValue('This is the answer to a multiple choice question');

answersAccessPackageAnswer1AnsweredQuestion = AccessPackageQuestion();
answersAccessPackageAnswer1AnsweredQuestion.set@odatatype('#microsoft.graph.accessPackageMultipleChoiceQuestion');

answersAccessPackageAnswer1AnsweredQuestion.setId('8fe745e7-80b2-490d-bd22-4e708c77288c');


answersAccessPackageAnswer1.setAnsweredQuestion($answersAccessPackageAnswer1AnsweredQuestion);
additionalData = [
'value' => 'MultipleChoiceAnswerValue', 
];
answersAccessPackageAnswer1.setAdditionalData(additionalData);



answersArray []= answersAccessPackageAnswer1;
answersAccessPackageAnswer2 = AccessPackageAnswer();
answersAccessPackageAnswer2.set@odatatype('#microsoft.graph.accessPackageAnswerString');

answersAccessPackageAnswer2.setDisplayValue('This is my answer.');

answersAccessPackageAnswer2AnsweredQuestion = AccessPackageQuestion();
answersAccessPackageAnswer2AnsweredQuestion.set@odatatype('#microsoft.graph.accessPackageTextInputQuestion');

answersAccessPackageAnswer2AnsweredQuestion.setId('7aaa18c9-8e4f-440f-bd5a-3a7ce312cbe6');


answersAccessPackageAnswer2.setAnsweredQuestion($answersAccessPackageAnswer2AnsweredQuestion);
additionalData = [
'value' => 'This is my answer to a text input question.', 
];
answersAccessPackageAnswer2.setAdditionalData(additionalData);



answersArray []= answersAccessPackageAnswer2;
request_body.setAnswers(answersArray);


assignment = AccessPackageAssignment();
additionalData = [
'accessPackageId' => '977c7ff4-ef8f-4910-9d31-49048ddf3120', 
];
assignment.setAdditionalData(additionalData);



request_body.setAssignment($assignment);


result = await client.identityGovernance.entitlementManagement.assignmentRequests.post(request_body);


```