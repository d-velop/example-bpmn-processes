[German](README_de.md)

# Exclusive gateway process

This process shows how an exclusive gateway can be modeled.

The variable `amount` must be transferred at the start of the process.
The process path is decided at the first gateway and depends on the value of the variable.
If the variable value is greater than 1000, the process follows the sequence flow `gateway-option-a` and a task with the subject "Hello World" is assigned to the user who started the process.
In the other case, the process follows the sequence flow `gateway-option-b` which does not have a meaning but is marked as default and the process is immediately finished.
