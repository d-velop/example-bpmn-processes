[German](README_de.md)

# Multi-instance process

This process shows how you can use multiple executions of a user activity.

The variable `performers` must be transferred at the process start.
This variable contains an array of identities.
A task is assigned to the corresponding users during the process.
As soon as each user has completed the task, the process is finished.
