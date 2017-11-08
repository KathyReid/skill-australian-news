# Australian News Skill

This skill reads the [Australian Broadcasting Network](http://abc.net.au) live radio news feed. The ABC is Australia's national public broacasting service.

The direct stream URLs from the ABC are at:
http://radio.abc.net.au/help/streams

Most of these streams are in *.pls* format, which is an XML playist format.

This skill currently plays the stream from:
http://live-radio02.mediahubaustralia.com/PBW/mp3/

This is a stream, not a recording, so when it plays it will begin mid-stream. ABC often streams the BBC World Service, with local Australian news updates on the hour.

## Current state

This Skill is **experimental**. It has been written to learn about Skills in Mycroft.

## Usage
* Speak: `Australian news`
* Speak: `Aussie news`
* Speak: `read the Australian news`

## Requirements

Nil

## Todo

In the future I would like to be able to do the following with this Skill:

* Implement support for *.pls* files by inspecting the *.pls* file, extracting the *.mp3* stream and playing it
* Implement support for more localised news stations, based on the User's geographic location. That is, play the ABC News Radio station for the capital city that is closest to the User's location. For example, if you're in Ballarat, play ABC Radio Melbourne. If you're in Dubbo, play ABC Radio Sydney. If you're in Katherine, play ABC Radio Darwin etc.
* Take a spoken parameter for city, and play the ABC News Radio station which is closes to this. Eg. `Play Aussie news Bathurst` -> would play ABC Radio Sydney.
* If I can find a pre-recorded *.mp3* or similar, then play this instead of a stream (had a look but couldn't find one)
