[German](README_de.md)

# Timer event process

This process shows how a timer event can be used.

At the start of the process, a task with the subject "Hello World" is assigned to the user who started the process.
If the user who started the process does not complete the task within one minute, the timer event is triggered.
The task is then deleted and the process follows the sequence flow `s3` to the end event.
