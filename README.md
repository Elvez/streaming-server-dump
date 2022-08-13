# streaming-server-dump

Here I put all the things I learnt or built about streaming servers.


## Resources

> http://live555.com/

> https://www.roborealm.com/help/RTSP_Player.php

> https://www.wowza.com/blog/streaming-protocols

> https://www.wowza.com/blog/hls-streaming-protocol

> https://www.wowza.com/blog/rtsp-the-real-time-streaming-protocol-explained

> https://gstreamer.freedesktop.org/documentation/gst-rtsp-server/rtsp-server.html?gi-language=c


## TCP vs UDP

> "Because UDP doesn’t support retransmissions, packet ordering, or error-checking, there’s potential for a network glitch to corrupt the data en route"

whereas,

> "TCP requires a three-way handshake when transporting data. The initiator (client) asks the accepter (server) to start a connection, the accepter responds, and the initiator acknowledges the response and maintains a session between either end"

> ![tcp VS UDP](https://user-images.githubusercontent.com/38424838/184505080-66984f98-c0ea-40ee-b6e6-481e92f79475.png)


## Miscellaneous

> ![OSI Model with units](https://user-images.githubusercontent.com/38424838/184504861-4932db92-ebce-40c1-94ab-b37326bb0c59.png)

> ![image](https://user-images.githubusercontent.com/38424838/184505293-99fcf542-4dd5-471b-a699-4c7386af1e9f.png)


### HLS (HTTP Live Streaming)

> ![image](https://user-images.githubusercontent.com/38424838/184507758-54a0cbec-c2ce-4afb-b016-a23eff499633.png)

> ![image](https://user-images.githubusercontent.com/38424838/184507821-6f68501b-c3d8-4c04-be0a-087959792ac9.png)

> ![image](https://user-images.githubusercontent.com/38424838/184507829-41ffacd4-7676-4d04-93d8-850c0d1cbe4b.png)

> #### .M3U8 Manifest File
"HLS video segments are indexed into a media playlist so that the video player understands how to organize the data. A master .m3u8 playlist file must also be created — think of this as the index of indexes — to instruct the player on how to jump between the variant-specific playlists. This is also referred to as the manifest file. Anyone delivering the stream can then distribute the content by embedding the .m3u8 reference URL in a web page or creating an application that downloads the file."
![image](https://user-images.githubusercontent.com/38424838/184507889-0fff0af0-67dc-4e5c-917e-2784e7d03e65.png)

