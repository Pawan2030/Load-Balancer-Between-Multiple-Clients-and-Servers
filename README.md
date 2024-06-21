# Load-Balancer-Between-Multiple-Clients-and-Servers

### Load Balancer with Round-Robin Algorithm

This project demonstrates a simple load balancer using the round-robin algorithm to distribute client requests across multiple servers. The setup includes three servers and six clients, all managed by a central load balancer.

## Project Structure

- `load_balancer/`
  - `load_balancer.cpp`: The load balancer that distributes client requests to the servers.
- `server/`
  - `server1.cpp`: Server 1 listening on port 8080.
  - `server2.cpp`: Server 2 listening on port 8081.
  - `server3.cpp`: Server 3 listening on port 8082.
- `client/`
  - `client1.cpp` to `client6.cpp`: Clients that connect to the load balancer.

## How to Run

### Servers

 Compile and run `server.cpp`:
   g++ -o server server/server.cpp -lws2_32
   ./server  
   [//]: # (for server1 server2 ... and so on....)
### Load Balancer
Compile and run load_balancer.cpp:
g++ -o load_balancer load_balancer/load_balancer.cpp -lws2_32
./load_balancer 

### Clients
Compile and run client.cpp:
g++ -o client client/client.cpp -lws2_32
./client  
[//]: # (for client1 , client2 ....and so on....)

### Example Output

https://github.com/Pawan2030/Load-Balancer-Between-Multiple-Clients-and-Servers/assets/136910101/45c8012d-80f8-48b6-b47f-c6dcbfa10ac4

### Future Scope
Database Integration:

Connect the servers to a database. Instead of serving static files, servers can fetch files from a database based on client requests and serve them dynamically.

### Advanced Load Balancing Algorithms:

Implement additional load balancing algorithms such as Least Connection, Weighted Response Time, etc., to optimize performance and resource utilization.

### Screenshots

![Screenshot (1)](https://github.com/Pawan2030/Load-Balancer-Between-Multiple-Clients-and-Servers/assets/136910101/054403f1-2cb0-4d9f-ab6d-e3687aa50169)![Screenshot (3)](https://github.com/Pawan2030/Load-Balancer-Between-Multiple-Clients-and-Servers/assets/136910101/7f9e15f7-26df-4a50-8167-235b95e751e7)
![Screenshot (2)](https://github.com/Pawan2030/Load-Balancer-Between-Multiple-Clients-and-Servers/assets/136910101/26edb12e-c4a1-432d-9973-727c72c1adf2)

### Create a new repository on GitHub and push your local repository to GitHub:

git remote add origin https://github.com/Pawan2030/my-load-balancer-project.git
git branch -M main
git push -u origin main


### Authors
# Pawan Mehta



