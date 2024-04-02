# CallonHit
Call on hit

**The Сoncept,**
Description of the principle of operation of the system

                       +-------------------------------+
+------------Device----| Accelerometer + on hit sensor |----------------+
|                      +----Sensitivity adjustment-----+                |
|   +-----+                                                             |
|   | GPS |            Sending duplicate data to                        |
|   +-----+            the SMS service                                  |
|      |                                                Radio Channel / |
|      |   +---------------------+                                   /  |
|      +-->| NMEA Protocol + CRC |                               /| /   |
|          +---------------------+                              / |/    |
|                 |                                            /        |
|                 |   +------------+                                    |
|                 +-->| DTMF Coder |                        \|/         |
|                     +------------+                         |          |
|                           |                                |          |
|                           |   |\    +------------+   +------------+   |
|                           +-->| +-->| Microphone |-->| GSM Module |   |
|                               |/    +------------+   +------------+   |
|                                                                       |
+-----------------------------------------------------------------------+


     Radio Channel /
                  /
+------------ /| / ------Supervisory Control And Data Acquisition-------+
|            / |/                                                       |
|           /                                                           |
|                                                                       |
|        \|/                                                            |
|         |            Or the use of a RESTful End-point,               |
|         |            API service                                      |
|   +------------+                                                      |
|   | GSM Module |                                                      |
|   +------------+                                                      |
|         |                                                             |
|         |   +---------+    /|   +--------------+                      |
|         +-->| Speaker |-->+ |-->| DTMF Decoder |                      |
|             +---------+    \|   +--------------+                      |
|                                        |                              |
|                                        |   +------+                   |
|                                        +-->| Data |                   |
|                                            +------+                   |
|                                               |                       |
|                                               |   +--------------+    |
|                                               +-->| PC Workspace |    |
|                                                   +--------------+    |
|                                                          |            |
|                                                          +            |
|                                                          |            |
|                                                    +------------+     |
|                                                    | GIS System |     |
|                                                    +------------+     |
|                                                                       |
+-----------------------------------------------------------------------+

p.s. It's simple enough to drop, shake or hit the phone..
