# Example Voting App

A simple distributed application running across multiple Docker containers.

## Architecture

![Architecture diagram](architecture.excalidraw.png)

* A front-end web app in [Python](/vote) which lets you vote between two options
* A [Redis](https://hub.docker.com/_/redis/) which collects new votes
* A [.NET](/worker/) worker which consumes votes and stores them in…
* A [Postgres](https://hub.docker.com/_/postgres/) database backed by a Docker volume
* A [Node.js](/result) web app which shows the results of the voting in real time

## Notes

The voting application only accepts one vote per client browser. It does not register additional votes if a vote has already been submitted from a client.

Here are screenshots of the project:

<img width="1511" alt="ss 1" src="https://github.com/user-attachments/assets/4b2646e9-b469-46c1-8c26-9da2e4185688" />
<img width="1512" alt="ss2" src="https://github.com/user-attachments/assets/a7888936-9ae3-412d-8919-8e57411e5492" />
<img width="1512" alt="ss3" src="https://github.com/user-attachments/assets/336936a6-7397-4c11-8633-3ec08e065b91" />
<img width="1512" alt="ss4" src="https://github.com/user-attachments/assets/aaff2ffd-aa4a-4164-bc42-528fc5ab756a" />
<img width="1512" alt="ss5" src="https://github.com/user-attachments/assets/c71a8fb8-9c14-4d16-8c4d-f6942f4347ff" />
<img width="1512" alt="ss6" src="https://github.com/user-attachments/assets/bbf82207-ae0f-452b-93d3-e98bd178077b" />
<img width="1512" alt="ss7" src="https://github.com/user-attachments/assets/01400eb6-5a49-49ba-bbdd-7c3b768d8cf2" />






