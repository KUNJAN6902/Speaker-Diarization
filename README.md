# Speaker-Diarization

## Part-1
</br>
Inputs : One audio files in wav format
</br>
Processing : The audio file has two speakers speaking to each other.  The input audio file should be split into two output audio file – in such a manner that each audio file has the audio speech of only one speaker. 
</br>
Outputs : Two audio files in wav format.  Each audio file should have the speech of one speaker alone. 
</br>
</br>
Following link contains information about various techniques/APIs/Frameworks available for Speaker Diarization:
</br>
=> https://wq2012.github.io/awesome-diarization/ </br>

</br>

Used : </br>
(1) DeepAffects API : https://docs.deepaffects.com/docs/speaker-diarization-api.html </br>
</br>
url = "https://proxy.api.deepaffects.com/audio/generic/api/v2/async/diarize" </br>
querystring = {"apikey":"XXXX", "webhook":"https://webhook.site/f5540c7c-b0ce-4a8c-9ad5-1aa1a8e03e90"}
</br>
</br>
(2) from pydub import AudioSegment

## Part-2
<br/>
Input: Audio file, in mp4 format, of a call center recording.  
<br/>
Recording Details : The recording has been done in stereo-channel format i.e. if you listen to this recording, using your headphones, you will see that one part of the conversation would be audible on your left ear – while the other part on your right ear.  
<br/>
Output :  The recording has to be split based on the two channels it has been recorded in.  As an output we need two audio recordings.  One recording will have the left channel input and the other output recording will have the right channel input.  It is important that both outputs are in WAV format.  
<br/>
<br/>
=> Function used to split file Channel wise<br/>
#Splitting Stereo Channels to Mono Channels<br/>
phone_call_channels = stereo_phone_call.split_to_mono()
<br/>
