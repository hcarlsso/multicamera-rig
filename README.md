# Cameras

Default is not use encrypted password

    rosrun axis_camera axis.py _hostname:=192.168.0.91 _password:=pass __ns:=/camera1/ _use_encrypted_password:=true

# IMU

Currently, rate is hardcoded in code. Rate is how fast the publisher publish?

    rosrun axis_imu axis_imu _frame_id:=imu_frame _rate:=100 _root_passwd:=pass _camera_ip:=192.168.0.91 _driver_ip:=192.168.0.1 _port:=5000 __ns:=/camera1/


# How to download the repo

Since there are submodules, a recursive clone has to be performed.

    git clone --recurse-submodules https://github.com/hcarlsso/multicamera-rig


# Applicability

The packages here are for the aptitude version of ROS, provided in Ubuntu. Since
it is not regularly updated, a lot of different packages has to be manually added.
Thus, I decided to skip this version of ROS, and go for the melodic version.
Think the version should be ROS lunar
