### Lab: Create a Dockerfile for Node.js App Deployment

#### Objective:
Create a Dockerfile to package a Node.js application for deployment using Visual Studio Code.

#### Prerequisites:
- Node.js installed on your machine.
- Docker installed on your machine.
- Visual Studio Code installed on your machine.

#### Steps:

1. **Open Visual Studio Code:**
   Open Visual Studio Code on your machine.

2. **Open your Node.js project:**
   Open the Node.js project for which you want to create a Dockerfile in Visual Studio Code.

3. **Create a new file:**
   Create a new file in the root of your project and name it `Dockerfile`. You can do this by right-clicking on the project folder, selecting "New File," and entering the name.

4. **Edit the Dockerfile:**
   Open the `Dockerfile` and add the following content:

   ```Dockerfile
   # Use an official Node.js runtime as a base image
   FROM node:14

   # Set the working directory in the container
   WORKDIR /usr/src/app

   # Copy package.json and package-lock.json to the working directory
   COPY package*.json ./

   # Install app dependencies
   RUN npm install

   # Copy the rest of the application code to the working directory
   COPY . .

   # Expose the port on which the app will run
   EXPOSE 3000

   # Define the command to run your application
   CMD ["npm", "start"]
   ```

   Adjust the Node.js version (`FROM node:14`) and the port (`EXPOSE 3000`) based on your application's requirements.

5. **Save the Dockerfile:**
   Save the `Dockerfile` by clicking on File > Save or using the keyboard shortcut (Ctrl + S).

6. **Build the Docker image:**
   Open the VS Code terminal and navigate to the project directory. Run the following command to build the Docker image:

   ```bash
   docker build -t your-image-name .
   ```

   Replace `your-image-name` with a suitable name for your Docker image.

7. **Verify the Docker image:**
   After the build completes, verify that the Docker image was created successfully by running:

   ```bash
   docker images
   ```

   You should see your newly created image in the list.

8. **Run the Docker container:**
   Run a Docker container based on the image you just created:

   ```bash
   docker run -p 3000:3000 your-image-name
   ```

   Replace `your-image-name` with the name you used in the build step.

9. **Access the Node.js app:**
   Open a web browser and navigate to http://localhost:3000. You should see your Node.js application running.

10. **Stop the Docker container:**
    Press `Ctrl + C` in the terminal where the container is running to stop it.

Congratulations! You have successfully created a Dockerfile for your Node.js application and deployed it using Docker. Adjust the instructions based on your specific project structure and requirements.