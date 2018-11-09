#update container state
RUN apt-get install ffmpeg

RUN apt-get update

RUN apt-get install ffmpeg

RUN pip install --upgrade youtube-dl

#This should be added to ENTRYPOINT, at least a variation of it :/
#youtube-dl -x --audio-format "mp3" --audio-quality 0 https://www.youtube.com/watch?v=z87ghOaL-WE

#youtube-dl -x -i --audio-format "mp3" -o %(title)s.%(ext)s --audio-quality 0 

