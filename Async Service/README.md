[German](README_de.md)

# Async service process

This process shows how an asynchronous external service is called.

The asynchronous service "Hello World" included in d.velop process serves as an example.
The service can be called using the URI `/process/services/helloworld/async`.
It expects an input variable called `yourName` and returns an output variable called `greeting` with the value "Hello <yourName>".

In this exemplary process, the "Hello World" service is called first.
The name of the user who started the process is used as the input variable `yourName`.
Afterwards, the process is halted until the server answers.
The output variable `greeting` received from the server is mapped to the process variable of the same name (`greeting`).
After calling the service, the process contains a process variable named `greeting` with the value "Hello <name of the user who started the process>".
This process variable is used as the name for the following user task, so that the process starter receives a task with the subject "Hello <name of the user who started the process>".
After completing the task, the process is finished.
