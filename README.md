# OpenAI Whisper API
Testing out the OpenAI Whisper API with a Finance use case. Here we're trying to compare SPY prices to Jerome Powell's Fed Rate Hike announcement.

**Whisper API**
Installation

```
!pip install -U openai-whisper
```

Importing
```
import whisper
```

Select Model
![whisper-models](https://user-images.githubusercontent.com/116864320/223668846-4763494d-c9bd-4655-92a7-8c026d2906ea.png)

```
model = whisper.load_model('base')

# do the transcription
output = model.transcribe("fed_meeting_trimmed.mp4")
```