# ros_install_tutorials

## description of CMakeLists.txt

`install`ディレクトリ以下に構成される
`${CATKIN_PACKAGE_LIB_DESTINATION}`: `lib`
`${CATKIN_PACKAGE_BIN_DESTINATION}`: `lib/<package name>`
`${CATKIN_PACKAGE_SHARE_DESTINATION}`: `share/<package name>`

## how to install
```
catkin_make install
```

catkin_workspaceに`install`ディレクトリが作成される

## how to run
```
roslaunch ros_install_tutorials ros_install_tutorials.launch
```

## output
```
catkin_ws/install
├── .catkin
├── .rosinstall
├── _setup_util.py
├── env.sh
├── include
│   └── ros_beginner_tutorials
├── lib
│   ├── pkgconfig
│   ├── python2.7
│   └── ros_install_tutorials
├── setup.bash
├── setup.sh
├── setup.zsh
└── share
    └── ros_install_tutorials
```

----

## FYI
init gen command
```
catkin_create_pkg ros_install_tutorials std_msgs roscpp
```

### catkin_make install
* [catkin/Tutorials/using\_a\_workspace \- ROS Wiki]( http://wiki.ros.org/catkin/Tutorials/using_a_workspace#Installing_Packages )
* [ja/catkin/Tutorials/using\_a\_workspace \- ROS Wiki]( http://wiki.ros.org/ja/catkin/Tutorials/using_a_workspace )

> なお，install space か devel spaceのどちらか一方を使うべきで，同時に両者を使うべきではありません．devel space は開発者自身で作成したワークスペース内のパッケージを開発する上で有効です．毎回 install を起動する必要がないからです． 

* [catkin\_make install \- ROS Answers: Open Source Q&A Forum]( https://answers.ros.org/question/259788/catkin_make-install/ )

* [ja/catkin/CMakeLists\.txt \- ROS Wiki]( http://wiki.ros.org/ja/catkin/CMakeLists.txt )
* [catkin/CMakeLists\.txt \- ROS Wiki]( http://wiki.ros.org/catkin/CMakeLists.txt )

### ros launch
* [ROS launchファイルの使い方]( https://kazuyamashi.github.io/ros_lecture/ros_launch.html )
* [【ROS】一斉にnodeを起動するLaunchの書き方 \- 極楽とんぼのロボット製作記]( https://www.g104robo.com/entry/ros-launch )
