# kitti2bag

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

