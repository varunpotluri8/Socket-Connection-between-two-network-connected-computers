# Socket-Connection-between-two-network-connected-computers
In this project, we will use a socket connection to emulate communication between two network-connected computers, say C1 and C2, and implement the following:
• Process P1, running on C1, has access to a text file, F1, of size 300 bytes. Process P2, running on C2, has access
to a text file, F2, also of size 300 bytes. The contents of these two text files are different.
• Either one of P1 or P2 initiates a socket connection with the other. 
• Once the connection is established, the two processes do the following (these are the project requirements):
– P1 should send the original contents of F1 to P2 using four messages with the first message containing the
first 75 bytes of F1, the next containing the next 75 bytes of F1 and so on.
– Similarly, P2 should send the original contents of F2 to P1 using three messages with the first message
containing the first 100 bytes of F1, the next containing the next 100 bytes of F1 and so on.
– P1 should append the information received from P2 to the end of F1.
– P2 should insert the information received from P1 in the beginning of F2.

Files F1 and F2 should be identical and of size 600 bytes. As we do not have access to two different file systems on two different machines, you will achieve the desired outcome as follows:
1. First create a subdirectory named D1, or some other name that isn’t already taken, in your home directory. Within that directory create the two files F1 and F2 of the desired size and contents.
2. Establish two connections . One of them will act as C1 and another as C2. Ideally, you would have two separate terminal windows, one in which you are logged into C1 and another in which you are logged into C2. 
3. Launch a socket server program that you will write as part of this project on C1. Now, C1 will be listening for incoming connection requests.
4. Next, launch the socket client program, also written by you as part of this project, on C2.
5. Have the client running on C2 establish a reliable socket connection (TCP) with the server running on C1.
6. Once the connection is established, implement the project requirements stated above.

When your processes terminate at both the machines, you should have two identical files F1 and F2 in the subdirectory D1 of your home directory.
