# Custom diff drive controller (plugin) package

## Changes and Current State
- The required changes have been made for deadband implementation in `src/diff_drive_controller.cpp`, lines `259-281`.
- Two new parameters are added: `linear_deadband` and `angular_deadband` in `src/diff_drive_controller_parameter.yaml`.
- The package builds successfully without any errors. If faced, resolve using rosdep.
- A dependency needed to be installed separately - realtime-tools, using `sudo apt install ros-humble-realtime-tools`.

## Work Needed!
- The packagen is not being identified by the ros2 system since the plugin needs to be exported a certain way. 
- The files `diff_drive_plugin.xml`, `package.xml` need looking into.
- Refer doc - http://wiki.ros.org/pluginlib for info on working on this task.
