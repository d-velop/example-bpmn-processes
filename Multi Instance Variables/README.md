[German](README_de.md)

# Multi-instance process with variables

This process shows how you can change variables in the process in a multi-instance of a subprocess.

The variable `allAssignees` must be transferred at the process start.
This variable contains an array of identities.
A task is assigned to the corresponding users during the process.
As soon as a user has finished his task and has assigned a value to the local variable `decision`, this value is written to the global variable `allDecisions`.
As soon as each user has completed the task, the process is finished.
