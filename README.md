# Restshell Example
An example extension of restshell where a new main package is created to host the shell of restshell. This mechanism is a recommended way to build a restshell with your own commands and keep the base contents. This repository includes the example commands to follow.

cd rs
go build

The build produces a new and different exe name and with the example commands included.

You can fork or copy this repository to build your own commands and tool.

# Example Commands
The example commands are examples of adding commands. Additional commands can be added to init.go or an init2.go (see restshell Readme). The init2.go is an example init file that can be used with the original restshell code base to add external commands. When creating a new main package new commands can be added to the init.go file directly.

# Test directory
The rs\tests folder contains tests that verify the function of the restshell command to verify operation with updates to the shell package..

Tests are run as follows:

cd rs
go build
./rs run tests\test

All assertions should pass when the script completes.
