# Backend

* The software can be created using QT libraries in *C++* or *Python*. 
* The server can be created using *Node.js* or *Python* libraries and to communicate betwween the servers and the clients, *WebSockets* can be used. 
* After the server and the database created, *Postman* can be used for the queries and the data tracking for debugging. 

In the backend part there is no restrictions. The developer has the full freedom. However detailed report needs to be handing over to the team leader.

---

### Data Storage

> Efficincy of the software and memory is the main problem when stroing data, so we recommend using hash tables with a hash function which gives the username can be used to store data. Using linked list in the hash table will increase the overall memory but it reduces the probability of collisions and it is also increase efficiency when adding new user to the database. However, if the database includes less than *x* (which is a threshold) data, circular or simple linked list with an iterator can be used also. We strongly recommend to do some benchmarking with *x* data to calculate the overall memory and time consume of both data structure and prepare a detailed report to calculate the threshold. After that when designing the software, firstly the linked list approach can be developed while the data below the threshold. When the data is bigger than the threshold, the server software can be updated to use hash table and function to store and provide the requested data to clients.

---

### Server Client Communications

> The clients sends server to the new user data when a new user is added and server has to send the new data to send back actual data to all of the clients. To prevent the race conditions mutexes and semaphores has to be used in the server and client side.


---

### Some Usefull Features

> Some useful features can be implemented in the client side. For example a sorting algorithm can be implemented to provide users the sorted data. For this purpose we use merge sort in this situation since it has the overall time complexity of O(nLogn) which is decent and reliable in worst case scenarios. 