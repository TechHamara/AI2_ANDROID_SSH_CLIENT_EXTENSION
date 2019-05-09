# AI2_SSH_EXTENSION:
Android client SSH extension for MIT Application Inventor 2


This is an AI2 extension made in Java for Android, compiled with the Apache ANT builder. It allows issuing Linux Bash/Shell commands to a remote SSH server, prefereably done in short execution, once the runnable thread runs under the AssyncTask, otherwise the whole application will become unresponsive to user interactions.

Bellow, a snapshot of the Component collection:

<img src="https://github.com/teprom/AI2_SSH_EXTENSION/blob/master/Component.png" alt="alt text" width="200" height="200">


# USAGE:


1 ) Fill string variables "SetUser", "SetHost" and "SetPasswords" accordingly, without queotes

2 ) Fill string variable "Command" with the Bash/Sheel command to be issued, without queotes (e.g: ls )

3 ) Call the function "SendData"

4 ) Get result either:

4.1 ) ...from within "NewIncomingMessage" event, argument "data" contains current text line, indded the last one.

4.1 ) ...by reading "GetReceivedMessage" variable; it is assyncronously updated (intermediary values are superseded)


# APPLICATION EXAMPLE:


A simple application with few components can be made to show check the extension working:

<img src="https://github.com/teprom/AI2_SSH_EXTENSION/blob/master/TestApp.png" alt="alt text" width="400" height="200">


With the suggested arrangement:

<img src="https://github.com/teprom/AI2_SSH_EXTENSION/blob/master/Screen.png?raw=true" alt="alt text" width="300" height="300">

