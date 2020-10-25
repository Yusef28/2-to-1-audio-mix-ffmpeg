# 2-to-1-audio-mix-ffmpeg

### One Liner:
`ffmpeg -i audio1.mp3 -i audio2.mp3 -filter_complex "amix=inputs=2:duration=shortest:dropout_transition=3:weights=3 1" -c:a libmp3lame zussamengefuhrt.mp3`
