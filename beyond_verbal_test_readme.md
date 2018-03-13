Beyond Verbal’s API analyzes the ACOUSTIC traits of utterances 
http://www.beyondverbal.com/api/

    * Sadness/Uncertainty/Boredom
    * Anger/Dislike/Stress
    * Neutral
    * Happiness/Enthusiasm/Friendliness
    * Warmth/Calmness

A key indicator of a speaker’s emotional state during the analyzed voice section, ranging from anger, sadness and neutrality to happiness and warmth

Valence is a variable which ranges from negativity to positivity. When listening to a person talk, it is possible to understand how “positive” or “negative” the person feels about the subject, object or event under discussion.

Arousal is a variable that ranges from tranquility/boredom to alertness/excitement. It corresponds to similar concepts such as level of activation and stimulation.

Temper is an emotional measure that covers a speaker’s entire mood range. Low temper describes depressive and gloomy moods. Medium temper describes friendly, warm and embracive moods. High temper values describe confrontational, domineering and aggressive moods.

Links
http://developers.beyondverbal.com/Home/Index
http://developers.beyondverbal.com/Home/api
https://github.com/BeyondVerbal-V3
https://github.com/BeyondVerbal-V3/Python

audio record
Recorded Audio in Quicktime, then opened with ITUNES then converted to WAV

first error WAV format
Ryans-MBP-4:Python ryan$ python BVC.py
{u'status': u'failure', u'reason': u'The API requires WAV PCM 8 KHz, 16 bit Mono'}
so went to itunes>preferences>general>import>WAV>Custom>8khz & 16bit mono

Each time manually updated file:

# audio_test_enthused_friendly.wav
yeah. Yeah thank you for taking my call. I need to change my phone number. My new number is 5551234. Yeah. And my new address is. 678 oak street. In Denver Colorado. Yes mmhm. Very yep. And yes I still have my ritual car. Very good thank you for helping me change that. By. 

{u'status': u'success', u'recordingId': u'43c8064e-a326-4df8-8c51-13dbf6d76990', u'result': {u'duration': u'34526.63', u'analysisSegments': [{u'duration': 13420, u'analysis': {u'Arousal': {u'Group': u'low', u'Value': u'7.23', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Valence': {u'Group': u'positive', u'Value': u'84.24', u'Summary': {u'Mode': u'positive', u'ModePct': 100}}, u'Temper': {u'Group': u'low', u'Value': u'8.59', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Vad': {u'Voiced': u'6.96'}, u'Mood': {u'Group11': {u'Primary': {u'Phrase': u'Loneliness, Unfulfillment', u'Id': 7}, u'Secondary': {u'Phrase': u'Loneliness, Unfulfillment', u'Id': 7}}, u'Composite': {u'Primary': {u'Phrase': u'Striving for love or belonging.', u'Id': 16}, u'Secondary': {u'Phrase': u'Fear of abandonment. Love and lack of self-confidence.', u'Id': 214}}, u'Group21': {u'Primary': {u'Phrase': u'loneliness', u'Id': 16}, u'Secondary': {u'Phrase': u'loneliness', u'Id': 16}}}}, u'offset': 16}, {u'duration': 14580, u'analysis': {u'Arousal': {u'Group': u'low', u'Value': u'1.20', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Valence': {u'Group': u'neutral', u'Value': u'37.21', u'Summary': {u'Mode': u'neutral', u'ModePct': 50}}, u'Temper': {u'Group': u'low', u'Value': u'8.04', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Vad': {u'Voiced': u'8.80'}, u'Mood': {u'Group11': {u'Primary': {u'Phrase': u'Loneliness, Unfulfillment', u'Id': 7}, u'Secondary': {u'Phrase': u'Loneliness, Unfulfillment', u'Id': 7}}, u'Composite': {u'Primary': {u'Phrase': u'Loneliness, fatigue, emotional frustration.', u'Id': 79}, u'Secondary': {u'Phrase': u'Striving for love or belonging.', u'Id': 16}}, u'Group21': {u'Primary': {u'Phrase': u'loneliness', u'Id': 16}, u'Secondary': {u'Phrase': u'loneliness', u'Id': 16}}}}, u'offset': 14826}], u'analysisSummary': {u'AnalysisResult': {u'Arousal': {u'Mode': u'low', u'ModePct': 100}, u'Valence': {u'Mode': u'neutral', u'ModePct': 50}, u'Temper': {u'Mode': u'low', u'ModePct': 100}}}, u'sessionStatus': u'Done'}}

# audio_test_angerdislike.wav
Yeah I need to change my address yeah. Yeah my number 2. No I don't. My new number is 5551234. No yes. My new address is 678. Come St. And yet I still got the car. Yeah okay thanks for help. By. 

{u'status': u'success', u'recordingId': u'31753631-f8f5-41fb-9d3b-08c34c7b9aa9', u'result': {u'duration': u'28698.38', u'analysisSegments': [{u'duration': 13790, u'analysis': {u'Arousal': {u'Group': u'low', u'Value': u'8.51', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Valence': {u'Group': u'negative', u'Value': u'15.19', u'Summary': {u'Mode': u'negative', u'ModePct': 100}}, u'Temper': {u'Group': u'low', u'Value': u'12.01', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Vad': {u'Voiced': u'6.15'}, u'Mood': {u'Group11': {u'Primary': {u'Phrase': u'Sadness, Sorrow', u'Id': 9}, u'Secondary': {u'Phrase': u'Defensivness, Anxiety', u'Id': 3}}, u'Composite': {u'Primary': {u'Phrase': u'Remorseful. Conflict of reason and passion.', u'Id': 121}, u'Secondary': {u'Phrase': u'Pain, vulnerability, need to fight.', u'Id': 40}}, u'Group21': {u'Primary': {u'Phrase': u'loneliness', u'Id': 16}, u'Secondary': {u'Phrase': u'unhappiness', u'Id': 21}}}}, u'offset': 16}, {u'duration': 14590, u'analysis': {u'Arousal': {u'Group': u'low', u'Value': u'5.62', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Valence': {u'Group': u'negative', u'Value': u'9.47', u'Summary': {u'Mode': u'negative', u'ModePct': 100}}, u'Temper': {u'Group': u'low', u'Value': u'13.97', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Vad': {u'Voiced': u'7.01'}, u'Mood': {u'Group11': {u'Primary': {u'Phrase': u'Sadness, Sorrow', u'Id': 9}, u'Secondary': {u'Phrase': u'Self-Control, Practicality', u'Id': 10}}, u'Composite': {u'Primary': {u'Phrase': u'Disappointment.', u'Id': 124}, u'Secondary': {u'Phrase': u'Restrained communication through self-control.', u'Id': 169}}, u'Group21': {u'Primary': {u'Phrase': u'unhappiness', u'Id': 21}, u'Secondary': {u'Phrase': u'self control', u'Id': 19}}}}, u'offset': 13816}], u'analysisSummary': {u'AnalysisResult': {u'Arousal': {u'Mode': u'low', u'ModePct': 100}, u'Valence': {u'Mode': u'negative', u'ModePct': 100}, u'Temper': {u'Mode': u'low', u'ModePct': 100}}}, u'sessionStatus': u'Done'}}

# audio_test_boredsad.wav (poor audio quality)
Yeah. On number. All. All. Yeah. Phone number. That is what we. Yeah don't. The money involved. Yeah. Thank you for help. 

{u'status': u'success', u'recordingId': u'dbfdd24c-e3a9-432c-8912-73945abb05bb', u'result': {u'duration': u'43698.50', u'analysisSegments': [{u'duration': 13260, u'analysis': {u'Arousal': {u'Group': u'low', u'Value': u'9.65', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Valence': {u'Group': u'neutral', u'Value': u'53.27', u'Summary': {u'Mode': u'neutral', u'ModePct': 100}}, u'Temper': {u'Group': u'low', u'Value': u'14.48', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Vad': {u'Voiced': u'4.65'}, u'Mood': {u'Group11': {u'Primary': {u'Phrase': u'Sadness, Sorrow', u'Id': 9}, u'Secondary': {u'Phrase': u'Loneliness, Unfulfillment', u'Id': 7}}, u'Composite': {u'Primary': {u'Phrase': u'Helplessness.', u'Id': 139}, u'Secondary': {u'Phrase': u'Striving for love or belonging.', u'Id': 16}}, u'Group21': {u'Primary': {u'Phrase': u'inferiority', u'Id': 15}, u'Secondary': {u'Phrase': u'loneliness', u'Id': 16}}}}, u'offset': 16}, {u'duration': 18250, u'analysis': {u'Arousal': {u'Group': u'low', u'Value': u'13.89', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Valence': {u'Group': u'neutral', u'Value': u'58.12', u'Summary': {u'Mode': u'neutral', u'ModePct': 100}}, u'Temper': {u'Group': u'low', u'Value': u'15.19', u'Summary': {u'Mode': u'low', u'ModePct': 100}}, u'Vad': {u'Voiced': u'4.43'}, u'Mood': {u'Group11': {u'Primary': {u'Phrase': u'Defensivness, Anxiety', u'Id': 3}, u'Secondary': {u'Phrase': u'Love, Happiness', u'Id': 8}}, u'Composite': {u'Primary': {u'Phrase': u'Pain, vulnerability, need to fight.', u'Id': 40}, u'Secondary': {u'Phrase': u'Love, possessiveness from insecurity.', u'Id': 412}}, u'Group21': {u'Primary': {u'Phrase': u'unhappiness', u'Id': 21}, u'Secondary': {u'Phrase': u'love', u'Id': 17}}}}, u'offset': 13826}], u'analysisSummary': {u'AnalysisResult': {u'Arousal': {u'Mode': u'low', u'ModePct': 100}, u'Valence': {u'Mode': u'neutral', u'ModePct': 100}, u'Temper': {u'Mode': u'low', u'ModePct': 100}}}, u'sessionStatus': u'Done'}}


