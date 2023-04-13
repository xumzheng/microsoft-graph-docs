---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationRubric()
request_body.displayName = 'Example Points Rubric'

description = EducationItemBody()
description.content = 'This is an example of a rubric with points'

description.ContentType(BodyType('text'))


request_body.description = description
levels_rubric_level1 = RubricLevel()
levelsRubricLevel1.displayName = 'Good'

levels_rubric_level1_description = EducationItemBody()
levelsRubricLevel1Description.content = ''

levelsRubricLevel1Description.ContentType(BodyType('text'))


levelsRubricLevel1.description = levelsRubricLevel1Description
levels_rubric_level1_grading = EducationAssignmentGradeType()
levelsRubricLevel1Grading.@odatatype = '#microsoft.graph.educationAssignmentPointsGradeType'

additionalData = [
'maxPoints' => 2,
];
levelsRubricLevel1Grading.additionaldata(additionalData)



levelsRubricLevel1.grading = levelsRubricLevel1Grading

levelsArray []= levelsRubricLevel1;
levels_rubric_level2 = RubricLevel()
levelsRubricLevel2.displayName = 'Poor'

levels_rubric_level2_description = EducationItemBody()
levelsRubricLevel2Description.content = ''

levelsRubricLevel2Description.ContentType(BodyType('text'))


levelsRubricLevel2.description = levelsRubricLevel2Description
levels_rubric_level2_grading = EducationAssignmentGradeType()
levelsRubricLevel2Grading.@odatatype = '#microsoft.graph.educationAssignmentPointsGradeType'

additionalData = [
'maxPoints' => 1,
];
levelsRubricLevel2Grading.additionaldata(additionalData)



levelsRubricLevel2.grading = levelsRubricLevel2Grading

levelsArray []= levelsRubricLevel2;
request_body.levels(levelsArray)


qualities_rubric_quality1 = RubricQuality()
qualities_rubric_quality1_description = EducationItemBody()
qualitiesRubricQuality1Description.content = 'Argument'

qualitiesRubricQuality1Description.ContentType(BodyType('text'))


qualitiesRubricQuality1.description = qualitiesRubricQuality1Description
criteria_rubric_criterion1 = RubricCriterion()
criteria_rubric_criterion1_description = EducationItemBody()
criteriaRubricCriterion1Description.content = 'The essay\'s argument is persuasive.'

criteriaRubricCriterion1Description.ContentType(BodyType('text'))


criteriaRubricCriterion1.description = criteriaRubricCriterion1Description

criteriaArray []= criteriaRubricCriterion1;
criteria_rubric_criterion2 = RubricCriterion()
criteria_rubric_criterion2_description = EducationItemBody()
criteriaRubricCriterion2Description.content = 'The essay\'s argument does not make sense.'

criteriaRubricCriterion2Description.ContentType(BodyType('text'))


criteriaRubricCriterion2.description = criteriaRubricCriterion2Description

criteriaArray []= criteriaRubricCriterion2;
qualitiesRubricQuality1.criteria(criteriaArray)


qualitiesRubricQuality1.weight = 50.0


qualitiesArray []= qualitiesRubricQuality1;
qualities_rubric_quality2 = RubricQuality()
qualities_rubric_quality2_description = EducationItemBody()
qualitiesRubricQuality2Description.content = 'Spelling and Grammar'

qualitiesRubricQuality2Description.ContentType(BodyType('text'))


qualitiesRubricQuality2.description = qualitiesRubricQuality2Description
criteria_rubric_criterion1 = RubricCriterion()
criteria_rubric_criterion1_description = EducationItemBody()
criteriaRubricCriterion1Description.content = 'The essay uses proper spelling and grammar with few or no errors.'

criteriaRubricCriterion1Description.ContentType(BodyType('text'))


criteriaRubricCriterion1.description = criteriaRubricCriterion1Description

criteriaArray []= criteriaRubricCriterion1;
criteria_rubric_criterion2 = RubricCriterion()
criteria_rubric_criterion2_description = EducationItemBody()
criteriaRubricCriterion2Description.content = 'The essay has numerous errors in spelling and/or grammar.'

criteriaRubricCriterion2Description.ContentType(BodyType('text'))


criteriaRubricCriterion2.description = criteriaRubricCriterion2Description

criteriaArray []= criteriaRubricCriterion2;
qualitiesRubricQuality2.criteria(criteriaArray)


qualitiesRubricQuality2.weight = 50.0


qualitiesArray []= qualitiesRubricQuality2;
request_body.qualities(qualitiesArray)


grading = EducationAssignmentGradeType()
grading.@odatatype = '#microsoft.graph.educationAssignmentPointsGradeType'


request_body.grading = grading



result = await client.education.me.rubrics.post(request_body = request_body)


```