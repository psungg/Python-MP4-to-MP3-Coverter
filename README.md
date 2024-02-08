# Python-MP4-to-MP3-Coverter

## Code

```python
pip install moviepy
```

```python
from moviepy.editor import *

mp4File = "Perfect Carrier Landing Step-by-Step BREAKDOWN.mp4"
mp3File = "Carrier Landing.mp3"

videoclip = VideoFileClip(mp4File)

audioclip = videoclip.audio
audioclip.write_audiofile(mp3File)
```
