# Generic CMake template.

Aufgabe 

### IO-Tests.  

You can create subfolders in `/tests/io_tests/`. These subfolders must match the name of a program you have created within the project. The tests fail, if the program is not yet build. You can implement multiple IO-Tests for a single executable, by adding `<xx>.in`, `<xx>.out` and `<xx>.err` files (`<xx>` is the matching test number, e.g. 01). If the program is implemented, every `<xx>.in` file is applied to the program as stdin and the created stdout of the program is matched with the `<xx>.out` file, as the created stderr is matched with the `<xx>.err`. The tests fail if the outputs don't match the requirements. 

### Devcontainer

A devcontainer configuration is provided to use this template from within github codespaces. An Ubuntu container was chosen, in which gcc/gdb/cmake and libcriterion (for testing) was added.

__TODO__:  
  This codespace will still ask you to choose a compiler kit, even if there is only one.
  
  The cmake extension is buggy and showing a configuration moved warning message every time a container starts. 
            

