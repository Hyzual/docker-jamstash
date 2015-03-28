# docker-jamstash

A Dockerfile for [Jamstash][jamstash]. Uses nginx.

Use the following command to run it on port 8001 of your host machine :

```bash
sudo docker run -d --name jamstash -p 8001:80 hyzual/jamstash
```

You can now connect to `http://yourhost:8001` and enjoy Jamstash.

## Jamstash

Jamstash is a HTML5 Music Player. It uses either [Subsonic][subsonic] or [Internet Archive][archive] as a source of audio files to stream.

Imagine you can stream all your music from home, to any device, where ever you are. That is Subsonic! Now imagine having a Web App to stream your music that is as beautiful and well designed as it is functional, that is Jamstash!

**What?**  

* HTML5 Music Streaming App for your Subsonic server
* Archive.org Browsing and Streaming of Live Music

**Features**  

* HTML5 Audio with Flash fallback (provided by the jPlayer library)
* Flexible Layout (will scale to whatever size your browser window is)
* Keyboard shortcuts (back, forward, play/pause, skip to artist, media keys)
* Playlist support (create new, add to existing, delete)
* Podcast support (includes description field on hover)
* Favorite/Starred support for Albums & Songs
* Shortcuts supported
* Easy installation (Chrome App or manual install)
* FF/Chome support (IE9 works but is a little rough around the edges)
* Light/Dark Theme
* Last.fm support
* Autopilot Mode (click one button and songs continue to play)
* AutoSave Mode (saves position and current playlist if you close or refresh your browser)
* Built with AngularJS

You will need a Subsonic server to be able to play your own music. Subsonic is a free, web-based media streamer, providing ubiquitous access to your music. Use it to share your music with friends, or to listen to your own music while at work. Please see [mschuerig's debian-subsonic image][docker-subsonic] for a Docker-ready Subsonic image to run alongside Jamstash.
## Ports

### 80

Web app port

### 443

HTTPS port

[jamstash]: http://jamstash.com
[subsonic]: http://www.subsonic.org
[archive]: https://archive.org
[docker-subsonic]: https://registry.hub.docker.com/u/mschuerig/debian-subsonic/
