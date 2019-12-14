# Chat-via-File
We have a file which name is Chat.Txt. This is an empty file. There are
two processes in this project. Both of them have the ability to write/read
the Chat.Txt. These processes communicate via this file. <br>
One-by-One synchronization is handled with <b>SIGUSR1</b> and <b>SIGUSR2</b> signal usage. <br>
The SIGUSR1 and SIGUSR2 used in cross operation (i.e. Both Processes (P1, P2)
starts in Pause. P1 signals P2 using SIGUSR1 to wake it up. P2 signals P1 using SIGUSR2
to wake it up.) They understand their status with using <b> "flag" </b> variable.
