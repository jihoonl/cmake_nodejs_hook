cmake_nodejs_hook
===============

Provides cmake hook to manipulate node modules

* catkin_npm_update_target()
* catkin_npm_update_once()

It invokes npm update update in source directory. 
Note that it is untested with install space

* Example
```
...
find_package(catkin REQUIRED cmake_nodejs_hook)

# Calling npm update every complilation
catkin_npm_update_target()

# Calling only once 
catkin_npm_update_once()

catkin_package()
...
``
