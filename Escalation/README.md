[German](README_de.md)

# Escalation process

This process shows how an escalation can be modeled.

If the user who started the process does not complete the task "Hello World" within one minute, the boundary timer event is triggered and the task is cancelled (see the exemplary process "Timer event").
The process now triggers the escalation event `throw_time_escalation`.
This event is linked with the start event `sub_start` of the sub process via the escalation definition `time_escalation` so that the sub process is started.
Within the sub process, a task with the subject "Escalation occurred" is assigned to the user who started the process.
