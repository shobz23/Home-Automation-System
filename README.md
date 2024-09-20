# Home-Automation-System
This project demonstrates the Command Pattern in Java, applied to a Home Automation System. The Command Pattern is used to encapsulate requests as objects, allowing you to parameterize methods with different requests, queue them, and log their execution.

# Key Features:
Command Pattern: Encapsulates commands like turning lights on/off as objects.
Invoker (RemoteControl): Stores and executes commands.
Receiver (Light): Executes the actual actions when the command is executed.
Design Pattern Used:
Command Pattern - The Command Pattern is useful when you want to decouple the object that invokes the operation from the object that performs the operation. It helps in scenarios like undo/redo, scheduling operations, or managing commands in queues.

# Project Structure
The code is structured into the following files:

Command.java - Interface defining the execute() method for all commands.
Light.java - Receiver class that contains the actual business logic (turning lights on and off).
LightOnCommand.java - Concrete command to turn on the light.
LightOffCommand.java - Concrete command to turn off the light.
RemoteControl.java - Invoker class that stores and executes commands.
Main.java - Testing class that demonstrates how commands are used.

# How It Works:
The Light is the receiver that performs the actual operations (turning on and off).
The Command interface defines a method execute() that is implemented by concrete commands (LightOnCommand and LightOffCommand).
The RemoteControl acts as an invoker. It stores the command and calls the execute() method to perform the operation.
You can set the command to LightOnCommand or LightOffCommand on the remote control and execute it.
