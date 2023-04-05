---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.set@odatatype('#microsoft.graph.educationRubricOutcome')

additionalData = [
'rubricQualityFeedback' => rubricQualityFeedback1 = ()
		rubricQualityFeedback1.setQualityId('9a145aa8-f3d9-43a1-8f77-5387ff0693f2')

rubricQualityFeedback1Feedback = Feedback()
		rubricQualityFeedback1Feedback.setContent('This is feedback specific to the first quality of the rubric.')

		rubricQualityFeedback1Feedback.setContentType('text')


rubricQualityFeedback1.setFeedback($rubricQualityFeedback1Feedback)

rubricQualityFeedbackArray []= rubricQualityFeedback1;
rubricQualityFeedback2 = ()
		rubricQualityFeedback2.setQualityId('d2331fb2-2761-402e-8de6-93e0afaa076e')

rubricQualityFeedback2Feedback = Feedback()
		rubricQualityFeedback2Feedback.setContent('This is feedback specific to the second quality of the rubric.')

		rubricQualityFeedback2Feedback.setContentType('text')


rubricQualityFeedback2.setFeedback($rubricQualityFeedback2Feedback)

rubricQualityFeedbackArray []= rubricQualityFeedback2;
request_body.setRubricQualityFeedback(rubricQualityFeedbackArray)


'rubricQualitySelectedLevels' => rubricQualitySelectedLevels1 = ()
	rubricQualitySelectedLevels1.setQualityId('9a145aa8-f3d9-43a1-8f77-5387ff0693f2')

	rubricQualitySelectedLevels1.setColumnId('4fb17a1d-5681-46c2-a295-4e305c3eae23')


rubricQualitySelectedLevelsArray []= rubricQualitySelectedLevels1;
rubricQualitySelectedLevels2 = ()
	rubricQualitySelectedLevels2.setQualityId('d2331fb2-2761-402e-8de6-93e0afaa076e')

	rubricQualitySelectedLevels2.setColumnId('aac076bf-51ba-48c5-a2e0-ee235b0b9740')


rubricQualitySelectedLevelsArray []= rubricQualitySelectedLevels2;
request_body.setRubricQualitySelectedLevels(rubricQualitySelectedLevelsArray)


];
request_body.setAdditionalData(additionalData)




result = await client.education.classes._by_id('educationClass-id').assignments._by_id('educationAssignment-id').submissions._by_id('educationSubmission-id').outcomes._by_id('educationOutcome-id').patch(request_body)


```