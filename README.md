# ROS2常用命令
1.创建
ros2 pkg create 包名 --build-type 构建类型 --dependencies 依赖列表 --node-name 可执行程序名
构建类型：ament_cmake(C++),ament_python(python)
依赖列表：不同的依赖可以用空格分割

2.编译
colcon build
或
colcon build --packages-select 功能包名

3.查找
输出所有功能包或指定功能包下的可执行程序：ros2 pkg executables [包名]
列出所有功能包：ros2 pkg list
列出功能包路径：ros2 pkg prefix 包名
输出功能包的xml文件内容：ros2 pkg ml

4.执行
ros2 run 功能包 可执行程序

