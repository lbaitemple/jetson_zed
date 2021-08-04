# jetson_zed (jetson nano 4G)

1. https://stereolabs.sfo2.cdn.digitaloceanspaces.com/zedsdk/3.5/ZED_SDK_Tegra_JP45_v3.5.1.run

```
wget https://stereolabs.sfo2.cdn.digitaloceanspaces.com/zedsdk/3.5/ZED_SDK_Tegra_JP45_v3.5.1.run
chmod +x ZED_SDK_Tegra_JP45_v3.5.1.run
./ZED_SDK_Tegra_JP45_v3.5.1.run
```

Install python3 lib for ZED
```
git clone https://github.com/stereolabs/zed-python-api
cd zed-python-api/src/
python3 setup.py install
```

Install ROS wrapper
```

cd ~/catkin_ws/src
git clone --recursive https://github.com/stereolabs/zed-ros-wrapper.git
cd ../
rosdep install --from-paths src --ignore-src -r -y
catkin_make_isolated

```
