# Speaker-Diarization

Here, I take an audio file as input and to speech-to-text transcription with diarization.  </br>
Later based on diarization time offsets, I am creating two seperate audio files from original audio file as input.

Used : </br>
(1) https://docs.deepaffects.com/docs/speaker-diarization-api.html </br>
url = "https://proxy.api.deepaffects.com/audio/generic/api/v2/async/diarize" </br>
querystring = {"apikey":"XXXX", "webhook":"https://webhook.site/f5540c7c-b0ce-4a8c-9ad5-1aa1a8e03e90"}
</br>
</br>
(2) from pydub import AudioSegment
