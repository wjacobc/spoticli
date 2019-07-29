# spoticli
Command line utility for controlling Spotify devices

## Features
- Play/pause active device playback locally or remotely using `p`, `play`, or `pause`
- Set active device volume using `vol`
- Get output of currently playing track using `np`
- Search for songs and albums using `search` or `s`
- Play specific songs or albums using `play query` or by sending the output of a `search`
- Skip to the next or previous songs using `next` and `previous`

**In development**:
- First-time usage script that sets the device the script is running on for seamless playback start, as well as the option to write Spotify username/developer data to disk rather than having to create a credentials file on your own.

## Installation
Requires spotipy, which can be installed using

`sudo pip install git+https://github.com/plamere/spotipy.git --upgrade`

Which is required to use the most recent features, since the `pip` version of spotipy is outdated.

Once that is installed, clone the repository and run using `python spoticli.py`, or alias to whatever you may find useful.

## Sample Commands
Display the currently playing track:

```
$ python spoticli.py np
Twenty One Pilots - My Blood
```

Pause playback on the active device:

```
$ python spoticli.py pause
Paused playback on jacob-pc
```

Set active device volume:

```
$ python spoticli.py vol 50
Set volume on jacob-pc to 50%
```
