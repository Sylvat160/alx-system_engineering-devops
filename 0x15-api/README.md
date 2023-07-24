### Background Context

Old-school system administrators typically rely on Bash scripting to build their scripts. While Bash can handle many tasks, it may become messy and less efficient compared to other programming languages. The new generation of system administrators, known as Site Reliability Engineers (SREs), are more like regular software engineers, but their focus is on managing systems rather than building products. A significant difference between SREs and their predecessors is that SREs possess knowledge beyond just Bash scripting.

APIs (Application Programming Interfaces) are a popular way to expose applications and datasets, often serving as the public-facing part of websites and micro-services. APIs allow outsiders to interact with the systems, accessing and modifying data. In this project, the goal is to access employee data through an API and organize and export it into different data structures using Python scripts.

Since this task is not well-suited for Bash scripting, Python will be the language of choice for building the scripts.

### Resources

Before proceeding with the project, it's essential to read or watch the following:

- "Friends don't let friends program in shell script": A humorous take on why Bash scripting might not be the best choice for certain tasks.
- What is an API: An explanation of what an API is and its purpose.
- What is an API? In English, please: An easy-to-understand explanation of APIs.
- What is a REST API: Understanding the concept of a RESTful API.
- What are microservices: An introduction to the concept of microservices in software architecture.
- PEP8 Python style: Following the Python style guide (PEP8) to write clean and readable code, which is highly appreciated in the industry.

### Learning Objectives

By the end of this project, you should be able to explain the following concepts to others without needing to rely on Google:

General:

- Identifying tasks that are not suitable for Bash scripting.
- Understanding what an API is and its purpose.
- Recognizing a REST API and its characteristics.
- Grasping the concept of microservices.
- Knowing the CSV and JSON data formats.
- Following Pythonic naming styles for packages, modules, classes, variables, functions, and constants.
- Understanding the significance of CapWords or CamelCase in Python.

### Copyright - Plagiarism

It's important to remember that you must come up with your own solutions to the project tasks to meet the learning objectives stated above. Copying and pasting someone else's work or publishing any content from this project is strictly prohibited and may result in removal from the program.

### Requirements

Ensure your code and project meet the following requirements:

General:

- Use the allowed editors: vi, vim, emacs.
- All Python files will be interpreted/compiled on Ubuntu 20.04 LTS using Python 3.8.5.
- All Python files should end with a new line.
- The first line of all Python files should be exactly "#!/usr/bin/python3".
- Organize imported libraries in alphabetical order.
- Include a README.md file at the root of the project folder.
- Your code should use pycodestyle (version 2.8.*) for adherence to the Python style guide.
- All your Python files must be executable.
- Test the length of your files using the "wc" command.
- All modules should have documentation that can be accessed using "python3 -c 'print(__import__("my_module").__doc__)'".
- Use "get" to access dictionary values by key, as it won't throw an exception if the key doesn't exist in the dictionary.
- Avoid executing code when imported by using "if __name__ == "__main__":"

