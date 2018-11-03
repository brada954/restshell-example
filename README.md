# Restshell Example
An example repository used to build a custom version of restshell with custom commands or functions. Restshell is modularized to simplify building of custom shells enabling developers to build shells with commands tailored to their custom applications or personal preferences. Forking or copying this repository is the recommended method to create a new repository to build a custom restshell using custom content. The new repository can be used to include your own custom content or reference other custom content in other repositories. Using this example will ensure custom shells will pickup new features and commands from the ever evolving restshell package. This repository includes example commands to follow.

There is no limit to the number of repositories that can be created with custom content that can be shared.

# Build instructions

cd rs
go build

The build produces a new restshell called rs.exe (or rs) which includes all the base functionality of restshell with the example commands loaded.

Run the following to see the help command
rs help

You can fork or copy this repository to build your own commands and executable.

# Example Commands
The example commands are examples of adding commands. Additional commands can be added to init.go or an init2.go (see restshell Readme). The init2.go is an example init file that can be used with the original restshell code base to add external commands. When creating a new main package new commands can be added to the init.go file directly.

# Tests
The rs\tests folder contains tests that verify the function of the restshell command to verify operation with updates to the shell package. The rs shell should be started from the tests folder to run the local .rsconfig file required by the tests.

Tests are run as follows:

cd rs
go build
cd tests
../rs run test

All assertions should pass when the script completes.
