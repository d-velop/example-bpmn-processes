[German](README_de.md)

# Hello world process

This process shows how user tasks can be modeled as "User Task" elements in a process.

If a process reaches a "User Task" element, a task is created in d.ecs task.
The value of the attribute `name` in the "User Task" element is the subject of the task.
Which user the task is assigned to is decided by the user assignment specified in the user task. Tasks are either assigned to a single user (camunda:assignee) or to multiple recipients (camunda:candidateUsers).

The current process consists of a single user task.
If the process is started, a task with the subject "Hello World" is created in d.ecs task.
This task is assigned to the user who started the process, because he is modeled as "camunda:assignee" in the user task with the process variable `dv_initiator`.
If the user who started the process completes the task, the process is finished.
