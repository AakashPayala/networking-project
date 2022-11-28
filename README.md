# networking-project

•	This is a simple game of tic-tac-toe developed in Python. It allows
two players to play with one another on different command lines
through networking. The server starts the game by first running
server.py, waiting for the client to connect by then running
client.py. Once they’re connected, the game itself starts.
The server starts as "X" and goes first, and the client is "O." The
players choose the square they would like to use with coordinates;
both "A1" and "1A" would be accepted, for example. The game
proceeds, with the players taking turns until one wins or the game is
a draw. The host, then the client, is asked whether they'd like a
rematch. If both agree, the game starts anew.
Socket programming is a way of connecting two nodes on a
network to communicate with each other. One socket(node) listens
on a particular port at an IP, while the other socket reaches out to
the other to form a connection. The server forms the listener socket
while the client reaches out to the server.


Rules of the game:

One by one the players have to enter a key ,‘O’ or ‘X’.A player can win the game when either of the diagonals have the same key i.e. ‘O’ or ‘X’ or any of the rows or the columns have the same key otherwise the game will result in a draw. 
                                 

Introduction


1. The client-server programming approach separates information producers from information users in a distributed computing system (servers). 

2. A client is a software programme that requests resources from a server, such as web pages or IP addresses. 

3. Clients can ask a server for this information whenever they want. Users of information are customers. 

4. A server is a programme that gives clients access to resources or information. It must be continuously operational and ready to respond to client requirements. 

5. Only server apps and their client counterparts can exchange data. Clients are not in direct contact with one another.
    
     6. Here, we have used python compiler to execute our code.

   7. Python is a multiprogramming language and it can be used for game development
Tic-Tac-Toe game is created using no extra libraries, but just socket          programming. 
 



               Requirement Analysis

From the given scenario, we draw the following requirements:
1. Identifying the appropriate hardware which would be used (Pycharm)
2. Users on the internet should be able to access the code .
3. Users on the internet should have access only to the public IP address of the server and not the private IP address.
4. The users in the organization should have full access to the server.
5. TCP/IP Network design with IP addressing
6. Features and configuration required on the hardware with explanation


ARCHITECTURE AND DESIGN
This is a sequence diagram that shows the timeline of events. It’s important to understand the flow before we start coding so make sure you understand the diagram completely.
Read through the points below if you are not familiar with Sequence Diagrams.
•	Time flows downward.
•	Arrows represent events. The start of an arrow denotes the Emitter, the end of an arrow denotes the listener. For example, Player1 emits the Create Game Event and the Socket Server listens to this event.
•	A rectangular box denotes waiting/processing time.
First, Player1 emits the create Game Event that the server acknowledges and responds back with a room ID.
Once, player2 emits join Game Event with the same room ID, the server then detects that both players have joined the room and shares the other player’s info with each other.














