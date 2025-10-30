This is an example ROS package for use in the HyperLabs ROS workshops.


## Build Steps
1. Make your workspace directory and go to the src directory
```
mkdir -p colcon_ws/src
cd colcon_ws/src
```
2. Acquire the source files. Clone this repository using git.
```
git clone https://github.com/Hyperloop-VCU/example-ros-package.git src/example-ros-package
```
3. Go back to the workspace directory
```
cd ..
```
4. Install the package's dependencies
```
rosdep install --from-paths src --ignore-src -r -y
```
5. Build the package using colcon
```
colcon build --symlink-install
```
6. Source the install source file to tell ROS about your new packages
```
source install/source.bash
```
