# File_Sharing

Blockchain/Other Technology: Collaboration platforms
Problem Statement:
        While we work on different site across globe, it is essential to enable all engineer to access the same engineering design file to work. There is a need to build a collaborative platform which will enable multi-site engineer to work on it while ensuring integrity, file transfer latency and security of the design documents  
Currently most of the teams have a global presence and the team members are spread across geographies. As the result work proceeds in a slow and disjointed manner when it comes to collaborative design, especially if multiple team members are working on the same design file. Archaic version control methods and lack of data availability can lead to rework, redesign, IP endangerment and added cost. There is a need to build a collaborative platform which will enable multiple team members to work on the same design file while maintaining security and a single source of truth throughout the life-cycle and protecting intellectual property.

#Project Name 
Secure File Transfer between Employees working at different locations of an organisation

## Table of Contents

- Requirements
     Administrator rights are required to install or update Visual Studio.
    .NET Framework 4.5.2 or above is required to install Visual Studio.
    .NET 4.8.1 is required to run Visual Studio on Windows 11 on Arm. 
     Universal Windows app development, including designing, editing, and debugging, requires Windows 10. 
     
     
- Recommended modules
      Socket.IO is a library that enables low-latency, bidirectional and event-based communication between a client and a server. It is built on top of the WebSocket protocol and provides additional guarantees like fallback to HTTP long-polling or automatic reconnection.
      
- Installation
    First please make sure to open your Visual Studio download and install. 
      https://visualstudio.microsoft.com/downloads/
      
## Configuration 
    Do the following configuration to start the server to send the files
      D:\Users\Desktop> mkdir fileshare
  D:\Users\Desktop> cd fileshare
  D:\Users\Desktop\fileshare> set-ExecutionPolicy RemoteSigned -Scope CurrentUser 
  D:\Users\Desktop\fileshare> npm init -y
Wrote to D:\Users\Desktop\fileshare\package.json:

{
  "name": "fsshare",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "node server.js",
    "start": "node server.js"
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "express": "^4.18.2",
    "socket.io": "^4.6.0"
  },
  "keywords": [],
  "devDependencies": {}
}


  D:\Users\Desktop\fileshare> npm install express socket.io --save

up to date, audited 78 packages in 708ms

7 packages are looking for funding
  run `npm fund` for details
found 0 vulnerabilities

  D:\Users\Desktop\fileshare> mkdir public       
  D:\Users\Desktop\fileshare> touch server.js    
    Touching server.js
  D:\Users\Desktop\fileshare> cd public          
  D:\Users\Desktop\fileshare\public> touch index.html   
Touching index.html
  D:\Users\Desktop\fileshare\public> touch code.js      
Touching code.js
  D:\Users\Desktop\fileshare\public> touch style.css    
Touching style.css
  D:\Users\Desktop\fileshare\public> touch receiver.html
Touching receiver.html
  D:\Users\Desktop\fileshare\public> touch receiver.js
Touching receiver.js
  D:\Users\Desktop\fileshare\public> cd..           
  D:\Users\Desktop\fileshare> npm start      

> fsshare@1.0.0 start
> node server.js

 {
  code: 'EADDRINUSE',
  errno: -4091,
  syscall: 'listen',
  address: '::',
  port: 5000
}

Node.js v18.14.1
  D:\Users\Desktop\fileshare>

## Sample Execution and output 
[Running process.pdf](https://github.com/sniwaserode/tri_nit_hackathon/files/10776446/Running.process.pdf)

![execution](https://user-images.githubusercontent.com/122344020/219937817-7db884ce-9479-4377-b48a-775fa15cae3d.png)


