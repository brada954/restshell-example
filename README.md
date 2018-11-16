# Restshell Example
The example repository demonstrates how to build a custom version of restshell with custom commands or functions. Similarly, repositories can be created to provide custom commands and functions to many custom restshells. Restshell becomes more powerful when it is built with custom commands and functions for developers particular applications and environments. 

It is recommended to copy or fork this repository to build a custom restshell with your custom content. Your custom restshell can also reference custom content in other repositories beyond the core features in restshell.

Following this example will ensure custom shells will pickup new features and commands from the evolving restshell package and other custom content repositories.

# Build instructions

```
cd rs
go build
```

The build produces a new restshell called rs.exe (or rs) which includes all the base functionality of restshell with the example commands loaded.

Run the following to see the help command
```
rs help
```

# Example Commands
The example commands are examples of adding commands. Additional commands can be added to init.go or an init2.go (see restshell Readme). The init2.go file enables custom content to be added without modifying the original init.go.

# Tests
The rs\tests folder contains tests that verify the function of the restshell command to verify operation with updates to the shell package. The rs shell should be started from the tests folder to run the local .rsconfig file required by the tests.

Tests are run as follows:

```
cd rs
go build
cd tests
../rs run test
```

All assertions should pass when the script completes.
