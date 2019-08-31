- Developed multi-threading servers in **C**
    - Monitored game resources and handle various types of requests from multiple clients (New Game,
    Reoconnect, Move, End) in the TCP thread; Used **select()** to deal with multitasking.
    - Replied to multicasting requests for failover in the UDP thread.
- Built the client to multicast for a new server or connect with the backup server while noting that the
original server crashes. Seamlessly resume the game from last move.