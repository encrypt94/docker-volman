docker-volman
=============

Just a simple script to mount volumes to docker running containers unmount and list them.
The cool code to mount a volume is taken "as is" from [this post](https://jpetazzo.github.io/2015/01/13/docker-mount-dynamic-volumes/) by @jpetazzo, kudos and cookies to him.

I don't know if this script works outside of my machine, i've written it for my own use, you should probably think twice before using it.

Usage
-----

** The script requires root access **

### Mount a volume

`docker-volman mount /path/to/host/volume:/path/to/container/volume container-id`

### Unmount a volume

`docker-volman unmount /path/to/container/volume container-id`

### List _all_ mounted volumes

`docker-volman list container-id`

Todo
----

* make possible to mount single files and not just directories
* make possible to mount stuff in read only mode
* cli parameters parsing just sucks