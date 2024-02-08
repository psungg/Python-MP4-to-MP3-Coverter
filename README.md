# Python-MP4-to-MP3-Coverter

## Code

```python
pip install pytube
```

```python
from pytube import YouTube

def YoutubeDownloader(link):
    youtubeObject = YouTube(link)
    youtubeObject = youtubeObject.streams.get_highest_resolution()
    try:
        youtubeObject.download()
    except:
        print("Some Errors Occurred")
    print("Done!",link)

#link = "https://www.youtube.com/watch?v=cr4IHJIyd_8"
link = input("Enter YouTube Link: ")
YoutubeDownloader(link)
```
