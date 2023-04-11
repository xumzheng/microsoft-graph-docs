---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Participant()
additionalData = [
'clientContext' => 'd45324c1-fcb5-430a-902c-f20af696537c', 
'participantMixerLevels' => participantMixerLevels1 = ()
		participantMixerLevels1.participant = '550fae72-d251-43ec-868c-373732c2704f'

		participantMixerLevels1.exclusive = true

participantMixerLevels1Ducking = Ducking()
		participantMixerLevels1Ducking.rampActive = 50

		participantMixerLevels1Ducking.rampInactive = 50

		participantMixerLevels1Ducking.lowerLevel = 10

		participantMixerLevels1Ducking.upperLevel = 50


participantMixerLevels1.ducking = participantMixerLevels1Ducking
sourceLevels1 = ()
		sourceLevels1.participant = '632899f8-2ea1-4604-8413-27bd2892079f'

		sourceLevels1.level = 50

		sourceLevels1.duckOthers = false


sourceLevelsArray []= sourceLevels1;
participantMixerLevels1.sourcelevels(sourceLevelsArray)



participantMixerLevelsArray []= participantMixerLevels1;
request_body.participantmixerlevels(participantMixerLevelsArray)


];
request_body.additionaldata(additionalData)




request_configuration = ParticipantRequestBuilderPostRequestConfiguration(
)


await client.communications.calls_by_id('call-id').participants_by_id('participant-id').post(request_body = request_body)


```