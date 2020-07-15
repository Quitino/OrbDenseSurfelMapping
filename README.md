##  readme
这是使用港科大的 DenseSurfelMapping + ORB-SLAM2测试的一个demo


run :
```bash
cd SURFELFUSION_ws/ &&
source devel/setup.bash && 
roslaunch surfel_fusion kitti_orb.launch

cd ORB_SLAM2/ &&
./orb_kitti_launch.sh

cd SURFELFUSION_ws/ && 
source devel/setup.bash &&
rviz src/surfel_fusion/rviz_config.rviz 


./kitti_publisher/src/KITTI/scripts/publisher.py

```

报错：
```
Framebuffer with requested attributes not available. 
Using available framebuffer. You may see visual artifacts.
```
- [参考](https://blog.csdn.net/weixin_42656998/article/details/99855639)

- [source repository](https://github.com/HKUST-Aerial-Robotics/DenseSurfelMapping)
