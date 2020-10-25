# 2-to-1-audio-mix-ffmpeg

### ffmpeg one-liner to merge two audio files with a 3:1 ratio:
`ffmpeg -i audio1.mp3 -i audio2.mp3 -filter_complex "amix=inputs=2:duration=shortest:dropout_transition=3:weights=3 1" -c:a libmp3lame mergedaudio.mp3`
