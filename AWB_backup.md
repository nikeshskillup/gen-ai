::page{title="Hands-on Lab: Write a Dockerfile for a Node app deployment"}

Estimate Time: 25 minutes

## Introduction
In this lab, you will explore how generative AI can assist in creating a Dockerfile for a Node.js application. You will utilize IBM\'s generative AI lab, powered by advanced language models. The goal is to generate the necessary code for the Dockerfile, simplifying the development of the Node.js application in a Docker environment.

## Objective
After completing this exercise, you will be able to:
- Acquire proficiency in utilizing ChatGPT for Dockerfile creation
- Develop effective questioning skills for Dockerfile creation inquiries
- Utilize IBM\'s generative AI lab to generate the necessary response for Dockerfile creation
- Ensure clarity and precision in providing details when seeking results from ChatGPT

Please note Generative AI is an evolving field. As you attempt the labs, your experience and output might differ from here.


::page{title="Prologue"}

#### What is a Dockerfile, and why use it?

A Dockerfile is like a recipe for your application\'s environment. It contains instructions that Docker uses to build a Docker image. This image, in turn, is a lightweight, standalone, and executable package that includes everything needed to run a piece of software, including the code, runtime, libraries, and system tools.

Dockerfiles are crucial in containerization, offering a standardized and reproducible way to package and deploy applications. They allow developers to encapsulate their applications and dependencies, ensuring consistent behavior across different environments. Dockerfiles simplify the development process and facilitates seamless collaboration and deployment.


::page{title="Step 1: Set up the AI classroom"}

The generative AI classroom allows you to write and compare your prompts to generate intended text with real-time chat responses.

You will have the generative AI classroom environment and instructions on one page in a browser. The instructions will be on the left of the screen, and the generative AI classroom will be on the right of the screen. You can interact with the language model using the message and chat fields.

Your AI Classroom will look similar to the screenshot shown below:

<img src="/images/setup_class.png" alt="AI Classroom overview">
<br><br>
To begin, configure your AI classroom to optimize your learning experience by following these steps:

#### 1. Name the chat
Click the pencil in the top-left corner to give your chat a name.

<img src="/images/chat_name.png" alt="name the chat">
<br><br>

#### 2. Choose the model
Go to the top-right corner and choose gpt-3.5-turbo from the drop-down for the text generation exercise. (By default, set to gpt-3.5.)

<img src="/images/choose_model.png" alt="choose model">
<br><br>

#### 3. Provide prompt instructions
Use the \"Prompt Instructions\" field in the upper right pane of the chat system to give instructions or specific details about the context of the required output. These instructions will be locked once the chat starts and cannot be modified later.

<img src="/images/prompt_instructions_box.png" alt="prompt instructions">
<br><br>

#### 4. Type your message
Use the text box at the end of the page to enter queries and converse with the chat system. Enter the following prompt to generate a Dockerfile, `Generate a Dockerfile for a Node.js application` and click `Start Chat`.

<img src="/images/prompt_message_box.png" alt="prompt message">
<br><br>


::page{title="Step 2: Start generating Dockerfile"}

Once your AI Classroom is ready, let\'s proceed and ask Generative AI for assistance writing a Dockerfile.

1. Enter the following question in the message box: `What is Dockerfile ?`

Now, view the AI\'s response for an explanation of a Dockerfile.

<img src="/images/what_dockerfile.png" alt="what is dockerfile">

<br><br>

2. Enter the following question in the message box: `What are the requirements for a Dockerfile?`

 Next, read the AI\'s response and proceed to ask questions about Dockerfile requirements.

<img src="/images/req_dockerfile.png" alt="requirements dockerfile">

<br><br>

3. Enter the following question in the message box: `What's the first crucial step when creating a Dockerfile for a Node.js application?`

 It is essential to understand the first step after selecting the base image for a Node.js Dockerfile.

<img src="/images/base_image.png" alt="base image">

<br><br>

4. Enter the following instructions in the message box: `Following the base image selection, Set the working directory inside the container to /app`

Then, you will learn about the next step to define the working directory inside the container.

<img src="/images/working_dir.png" alt="working directory ">

<br><br>

5. Enter the following instructions in the message box: `As selected working directory /app, bring the package.json and package-lock.json  to the working directory`

After that, you will understand the process of bringing package files into the working directory.

<img src="/images/package.png" alt="package.json and package-lock.json">

<br><br>


::page{title=""}


6. Enter the following questions in the message box: `Now, how do I install dependencies? And copy the remaining application code to the working directory?`

You will then get guidance on installing dependencies and copying the remaining application code.

<img src="/images/install_dependencies.png" alt="install dependencies">

<br><br>

7. Enter the following question in the message box: `Node.js app needs to be accessible on a specific port. What Dockerfile instruction do you include for this purpose?`

Then, you will learn the instructions to include for exposing a specific port.

<img src="/images/expose_ports.png" alt="Expose Port">

<br><br>

8. Enter the following question in the message box: `How to specify the command to start the Node.js application using CMD?`

After that, you will understand the final step in specifying the command to start the Node.js application.

<img src="/images/start_cmd.png" alt="Start Command">

<br><br>

9. Enter the following instructions in the message box: `Combine all the steps to form a complete Dockerfile for a Node.js application`

Now, you have completed all of the steps so you can view the generated Dockerfile.

<img src="/images/complete_dockerfile.png" alt="complete Dockerfile">

<br><br>

## Congratulations!

You have leveraged generative AI and developed a complete Dockerfile for a Node.js application.


::page{title="Summary"}


In this lab, you leveraged generative AI to simplify the creation of a Dockerfile for a Node.js application. You did this by interacting with the AI in the designated classroom and addressing key questions and steps involved in Dockerfile development. The generated Dockerfile serves as a foundation for deploying Node.js applications in a containerized environment. This experience showcases the potential of generative AI in enhancing the efficiency of Docker-based development workflows. Through guided interactions, you and othere can gain valuable insights into the Dockerfile creation process, making it more accessible and practical for real-world application deployments.


## Author(s)
Nikesh Kumar
Pallavi Rai


## Changelog
| Date | Version | Changed by | Change Description |
|------|--------|--------|---------|
| 2023-12-13 | 0.2 | Mary Stenberg| QA pass with edits |
| 2023-12-08 | 0.1 | Nikesh Kumar | Initial version created |
