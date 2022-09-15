 This is a full-fledged socket-client application. This application is written in the python language. 
 It uses socket programming principles and OS APIs to create a network that enables file transfer and command execution between a server and a client. 
 It has a custom encryption layer that enables three modes of encryption:
 Plain Text, Caeser Cipher, Transpose (text reversal) 
 The TCP is used as the transport layer protocol. 
 
 How to run the appliaction?
 ->Download and run the server.py and client.py files. They may/maynot be present on the same machine. (I had both of them on the same machine and handled them through different terminals). 
 
 What are the requests supported by the server?
  -> LS: It sends a list of all the files in the current directory of the server. 
  -> CD <dir>: Client can use this request to change the directory of the server. 
  -> CWD: server responds by sending the current working directory path to the client. 
  -> UPD <filepath>: client can upload any file (.txt, .png) to the working directory of the server.
  -> DWD <file path>:client can request for any file (.txt, .png) from the server and download it in it's working directory
  -> BYE: This command by the client terminates the connection between the hosts. The server.py and client.py files terminate. 
          For any further communication, re-run both the server and the client.
 
 The test files folder contains some of the test files that I used to de-bug the application. 
