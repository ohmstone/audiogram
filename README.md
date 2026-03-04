# Audiogram

One page offline webapp to create an audiogram (audio content as social media
video) for linkedin.

Main repo: [audiogram](https://github.com/ohmstone/audiogram)

## Purpose

To help create an eye-catching video from an audio file with optional text
(either force-aligned or not).

## How to use

This is a single file browser app. It doesn't have any server interaction. Go to
the link in this repo to start using it immediately.

You can also clone this repo and serve with a local web server.

**Example server:**

```python
python3 -m http.server 8000
```

## Capabilities

- [x] Add profile image to video
- [x] Add name to video
- [x] Add role / skills to video
- [x] Create video from audio (e.g. your voice)
- [x] Create nice visuals for audio
- [x] Customize audio visual colors
- [x] Optionally add text (e.g. transcript) to video
- [x] Use whisper style aligned transcription
- [x] Use unstructrured text transcription
- [x] Control word chunk and pacing of unstructured text
- [x] Preview video in real-time - no waiting
- [x] Create recording of video - high resolution output
- [x] Completely free, no sign up, completely offline
- [x] A safe and secure web-app, no downloads, any platform

## Further tooling

### Transcription with timings (aka forced-alignment)

If you have some recorded audio that you want to transcribe, I recommend using
[Whisper.cpp](https://github.com/ggml-org/whisper.cpp). It involves setup, and I
recommend using the largest model for greater accuracy.

### Text-to-Speech (TTS) and voice cloning

TTS helps if you have a script but don't have a decent microphone (or quiet
room), don't enjoy recording yourself, or would rather not use your natural
voice. I have ported a version of
[pocket-tts](https://github.com/kyutai-labs/pocket-tts) to Deno to run as a
local server. Just record a sample of a voice or use one of the provided voices,
provide the text you want to have generated, and that's it.

Get TTS here: [pocket-tts-deno](https://github.com/ohmstone/pocket-tts-deno).
You can also run the browser version of this, which is where I ported it from:
[pocket-tts-server](https://github.com/ai-joe-git/pocket-tts-server).

## Contributing, Disclaimer, and License

I used Claude to build this web-app. I only guided it and barely reviewed the
code. Use at your own risk, don't use in production without reviewing the code.

The code is licensed under MIT.

Any contributions are welcome but I probably won't do much more to improve this
as it gets the job done. I encourage you instead to fork it and make your own
variation for your own needs.
