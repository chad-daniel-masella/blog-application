# Steps In Creating Application:

## Setup Directory

Execute below commands via terminal

``` 
mkdir myapp

cd myapp
``` 

## Install Node.js Framework

``` 
npm init
``` 

#### You should have a project structure similar to the below:

``` 
.
├── README.md
├── app.js
├── node_modules
├── package-lock.json
└── package.json
```

## Starting Up Your Application

#### Run the following command via terminal from the project root directory

``` 
node app
```

[//]: # (This section included issues picked up while setting up my project)
# Solutions To Problems Encountered While Setting Up Project
## How To Kill Local Ports

### Option 1: Killing Multiple Ports

#### Mac OS:
```  
npx kill-port ${port1} ${port2} ${port3} 
```

### Option 2: To Kill Single Ports:

#### Linux/Mac OS:

``` 
$ sudo lsof -i tcp:3000
$ sudo kill -${PID_VALUE} PID
```

#### Windows OS:

```
netstat -ano | findstr :3000
tskill typeyourPIDhere 
```