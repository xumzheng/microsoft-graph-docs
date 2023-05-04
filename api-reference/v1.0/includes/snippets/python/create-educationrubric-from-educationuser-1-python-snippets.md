---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Education_rubric()
request_body.display_name = 'Example Credit Rubric'

description = Education_item_body()
description.content = 'This is an example of a credit rubric (no points)'

description.contenttype(BodyType.Text('bodytype.text'))


request_body.description = description
levels_rubric_level1 = Rubric_level()
levels_rubric_level1.display_name = 'Good'

levels_rubric_level1description = Education_item_body()
levels_rubric_level1description.content = ''

levels_rubric_level1description.contenttype(BodyType.Text('bodytype.text'))


levels_rubric_level1.description = levels_rubric_level1description

levelsArray []= levelsRubricLevel1;
levels_rubric_level2 = Rubric_level()
levels_rubric_level2.display_name = 'Poor'

levels_rubric_level2description = Education_item_body()
levels_rubric_level2description.content = ''

levels_rubric_level2description.contenttype(BodyType.Text('bodytype.text'))


levels_rubric_level2.description = levels_rubric_level2description

levelsArray []= levelsRubricLevel2;
request_body.levels(levelsArray)


qualities_rubric_quality1 = Rubric_quality()
qualities_rubric_quality1description = Education_item_body()
qualities_rubric_quality1description.content = 'Argument'

qualities_rubric_quality1description.contenttype(BodyType.Text('bodytype.text'))


qualities_rubric_quality1.description = qualities_rubric_quality1description
criteria_rubric_criterion1 = Rubric_criterion()
criteria_rubric_criterion1description = Education_item_body()
criteria_rubric_criterion1description.content = 'The essay\'s argument is persuasive.'

criteria_rubric_criterion1description.contenttype(BodyType.Text('bodytype.text'))


criteria_rubric_criterion1.description = criteria_rubric_criterion1description

criteriaArray []= criteriaRubricCriterion1;
criteria_rubric_criterion2 = Rubric_criterion()
criteria_rubric_criterion2description = Education_item_body()
criteria_rubric_criterion2description.content = 'The essay\'s argument does not make sense.'

criteria_rubric_criterion2description.contenttype(BodyType.Text('bodytype.text'))


criteria_rubric_criterion2.description = criteria_rubric_criterion2description

criteriaArray []= criteriaRubricCriterion2;
qualities_rubric_quality1.criteria(criteriaArray)



qualitiesArray []= qualitiesRubricQuality1;
qualities_rubric_quality2 = Rubric_quality()
qualities_rubric_quality2description = Education_item_body()
qualities_rubric_quality2description.content = 'Spelling and Grammar'

qualities_rubric_quality2description.contenttype(BodyType.Text('bodytype.text'))


qualities_rubric_quality2.description = qualities_rubric_quality2description
criteria_rubric_criterion1 = Rubric_criterion()
criteria_rubric_criterion1description = Education_item_body()
criteria_rubric_criterion1description.content = 'The essay uses proper spelling and grammar with few or no errors.'

criteria_rubric_criterion1description.contenttype(BodyType.Text('bodytype.text'))


criteria_rubric_criterion1.description = criteria_rubric_criterion1description

criteriaArray []= criteriaRubricCriterion1;
criteria_rubric_criterion2 = Rubric_criterion()
criteria_rubric_criterion2description = Education_item_body()
criteria_rubric_criterion2description.content = 'The essay has numerous errors in spelling and/or grammar.'

criteria_rubric_criterion2description.contenttype(BodyType.Text('bodytype.text'))


criteria_rubric_criterion2.description = criteria_rubric_criterion2description

criteriaArray []= criteriaRubricCriterion2;
qualities_rubric_quality2.criteria(criteriaArray)



qualitiesArray []= qualitiesRubricQuality2;
request_body.qualities(qualitiesArray)





result = await client.education.me.rubrics.post(request_body = request_body)


```