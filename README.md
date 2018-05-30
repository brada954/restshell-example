# Restshell Example
An example extension of restshell

cd rs
go build

The rs.exe file is an example of restshell compiled with a new main package and different exe name and with the example commands included.

# Example Commands
The example commands are examples of adding commands. Additional commands can be added to init.go or an init2.go (see restshell Readme). The init2.go is an example init file that can be used with the original restshell code base to add external commands. When creating a new main package new commands can be added to the init.go file directly.

# Test directory
The rs\tests folder contains tests that verify the function of the restshell command to verify operation with updates to the shell package..

Tests are run as follows:

cd rs
go build
./rs run tests\test

All assertions should pass when the script completes.
