# BPMWS24Prak-Lehre

## Intro

This project introduces a comprehensive web application built on the MERN (MongoDB, Express, React, Node.js) stack, tailored for customizable label printing with seamless integration of a DYMO PNP LabelManager. The primary objective is to provide users with a robust platform where they can effortlessly create, customize, and print labels according to their specific requirements.

The application architecture is divided into two main components: a Node.js backend serving as the server-side logic and API endpoints, and a React frontend offering an intuitive user interface for label customization and management. Additionally, a local server component facilitates the direct connection to a DYMO PNP LabelManager device for printing commands.


## Deployment

The frontend is already deployed on the [lehre server](https://lehre.bpm.in.tum.de/). To deploy the remote server and local server of the project, follow these steps:

### Local server

Clone this project to your local machine:

```bash
git clone https://github.com/niclasgrunau/dymo-pnp-local.git
```

Navigate to the root directory of the project and start local server:

```bash
cd dymo-pnp-local
node localServer.js
```

### Remote server

#### Connected to initial directory

If you are able to run "npm start" on [https://lehre.bpm.in.tum.de/~ge83neb/dymo-pnp/backend/](https://lehre.bpm.in.tum.de/~ge83neb/dymo-pnp/backend/) while being conected to the lehre server, the web application will run [on the server port](https://lehre.bpm.in.tum.de/ports/6982/) and [here](https://lehre.bpm.in.tum.de/~ge83neb/dymo-pnp/frontend/build/). If not, follow the steps below.

#### Else

First, connect via SSH to the [lehre server](https://lehre.bpm.in.tum.de/) and change to a directory where you want to save the project.

Then, clone this project to your server index:

```bash
git clone https://github.com/niclasgrunau/dymo-pnp.git
```

Navigate to the root directory of the project and install dependencies:

```bash
cd dymo-pnp
npm install
```

Then, navigate to the backend directory and install backend dependencies:

```bash
cd backend
npm install
```

Next, navigate to the frontend directory and install frontend dependencies:

```bash
cd ../frontend
npm install
```

For deploying, navigate to the frontend directory and create a static build of the frontend:

```bash
npm run build
```

Lastly, navigate to the backend directory and start the server:

```bash
cd ../backend
npm start
```




Navigate to the backend and start it:

```bash
cd dymo-pnp/backend
npm start
```



