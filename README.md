# waddle-bot
a discord bot made in python

test commit

## Dependencies
* discord.py - https://discordpy.readthedocs.io/en/latest/intro.html#installing

### Authors
* Nishant Arora
* JD Pappas

---
## Notes:

* Music streaming
    * Spotify playlists (-wb play \<URI\>)
        * get a Spotify playlist url (copy->share->get URI)
        * query Spotify API to get a dump of all playlist data
               * track name
               * artist
         * make a map of track name -> artist
         * go through each tuple and query youtube api of "track + artist"
         * grab 1st result
         * stream audio
    * Apple music playlists 
        * no idea this is all you JD
    * Player
        * Queue (data structure - ordered) [gets cleared on exit]
            * Simple array in python - https://www.geeksforgeeks.org/queue-in-python/
        * Song state - isPlaying, hasPlayed, positionInQueue
        * Not dump data to chat, not get limited. 
        * Pause, Play, Skip
        * Interaction
            * List queue
            * Remove from queue (by rank)
            * Add to top of queue


#### Look Into:
* (2) python poetry -> creating a project + venv
* (4) black, autopep8
* (5) pylint, flake8
* (6) precommit
* (1) pyenv
* (7) mypy -> typechecker
* (3) pytest

