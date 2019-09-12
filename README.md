Install nginx and the rtmp module

make a script like this:

    #!/bin/bash

    ffmpeg -i rtmp://10.5.40.101:1935/live/show -f null - 2>/dev/null &

That will be the client that fires up the rtmp stream

Now with your favorite player goto:

    http://nginx.ip:8080/live/view/index.m3u8

Happy watching...
