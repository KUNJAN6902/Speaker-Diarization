# Speaker-Diarization
</br>
Inputs : One audio files in wav format
</br>
Processing : The audio file has two speakers speaking to each other.  The input audio file should be split into two output audio file – in such a manner that each audio file has the audio speech of only one speaker. 
</br>
Outputs : Two audio files in wav format.  Each audio file should have the speech of one speaker alone. 
</br>

Used : </br>
(1) https://docs.deepaffects.com/docs/speaker-diarization-api.html </br>
url = "https://proxy.api.deepaffects.com/audio/generic/api/v2/async/diarize" </br>
querystring = {"apikey":"XXXX", "webhook":"https://webhook.site/f5540c7c-b0ce-4a8c-9ad5-1aa1a8e03e90"}
</br>
</br>
(2) from pydub import AudioSegment
