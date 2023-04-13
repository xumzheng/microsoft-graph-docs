---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Participant()
additionalData = [
'clientContext' => 'd45324c1-fcb5-430a-902c-f20af696537c', 
'participantMixerLevels' => participant_mixer_levels1 = ()
		participantMixerLevels1.participant = '550fae72-d251-43ec-868c-373732c2704f'

		participantMixerLevels1.exclusive = True

participant_mixer_levels1_ducking = Ducking()
		participantMixerLevels1Ducking.ramp_active = 50

		participantMixerLevels1Ducking.ramp_inactive = 50

		participantMixerLevels1Ducking.lower_level = 10

		participantMixerLevels1Ducking.upper_level = 50


participantMixerLevels1.ducking = participantMixerLevels1Ducking
source_levels1 = ()
		sourceLevels1.participant = '632899f8-2ea1-4604-8413-27bd2892079f'

		sourceLevels1.level = 50

		sourceLevels1.duck_others = False


sourceLevelsArray []= sourceLevels1;
participantMixerLevels1.sourcelevels(sourceLevelsArray)



participantMixerLevelsArray []= participantMixerLevels1;
request_body.participantmixerlevels(participantMixerLevelsArray)


];
request_body.additionaldata(additionalData)





await client.communications.calls_by_id('call-id').participants_by_id('participant-id').post(request_body = request_body)


```