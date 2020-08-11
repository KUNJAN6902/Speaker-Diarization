# Speaker-Diarization
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
