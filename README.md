# KITTI-Odometry to ROS bag

**This sourced code is for converting data of [KITTI odometry dataset](https://www.cvlibs.net/datasets/kitti/eval_odometry.php) to ROS bag format.**

1. Installation dependency

> GCC >= 5.4.0
>
> Cmake >= 3.0.2
> 
> [Eigen3](http://eigen.tuxfamily.org/index.php?title=Main_Page) >= 3.2.8
>
> [PCL](https://pointclouds.org/downloads/) == 1.7 for Ubuntu 16.04, and == 1.8 for Ubuntu 18.04
>
> [OpenCV](https://opencv.org/releases/) == 2.4.9 for Ubuntu 16.04
>
> [ROS](http://wiki.ros.org/ROS/Installation)

2. Create a new ROS workspace

```
mkdir /kitti2bag/src
cd /kitti2bag/src
```

3. Clone and build this repository

```
git clone https://github.com/ZikangYuan/kitti2bag.git
cd ..
catkin_make
```

4. Adjust directory structure

Please make sure that the directory format of KITTI is as follow:

```
KITTI 
├──────────00
           ├─────times.txt
           ├─────image_0
                 ├─────────000000.png
                 ├─────────000001.png
                 ├─────────......
                 └─────────004540.png
           └─────velodyne
                 ├─────────000000.bin
                 ├─────────000001.bin
                 ├─────────......
                 └─────────004540.bin
├──────────01
├──────────02
├──────────......
└──────────21
```

5. Run

```
source devel/setup.bash
roslaunch kitti2bag kitti2bag.launch
```

Please change the varibales about PATH in launch file before running.
