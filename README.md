# **ROS2_First_Step**
- Gazebo 상에서 camera 구현을 목표로 진행함
- 블로그를 참조해서 진행함 https://with-rl.tistory.com/
- 가장 많은 문제를 일으켰던 것은 이전에 다른 공부를 위해 설치해둔 패키지와 충돌하면서 Gazebo가 실행되지 않음
  ERROR : Exit code -6, 2 등등 나타남
- 또 다른 문제로 colcon build 시 --symlink-install을 하게 되는데 이렇게 하면 디렉토리 불러올 때 오류 발생했음
  -> 이는 그냥 colcon build로 해결 가능
- 블로그에 패키지 이름 오타 있음 (test -> tutorial)
<br/>
<br/>

# **Gazebo에서 카메라 구현하기**

# **Implementing a Camera in Gazebo**

- First terminal


```
cd ws/ros_ws
colcon build
source install/setup.bash
ros2 launch urdf_tutorial camera.launch.py world:=src/urdf_tutorial/config/with_robot.world
```
- If you want to customize the world, replace with_robot.world in /src/urdf_tutorial/config after customizing it.


![Image](https://github.com/user-attachments/assets/e4c83abd-4975-4013-8eb0-60d75e18748f)

<br/> 
<br/> 

# **추가적으로 rviz2 연동**

# **Additionally, rviz2 integration**

- Second terminal
  
```
cd ws/ros_ws
source install/setup.bash
rviz2
```

- After this, add RobotModel, LaserScan and Camera

![Image](https://github.com/user-attachments/assets/617f15ea-d44a-465d-85ee-144c6356b654)

<br/> 
<br/> 

# **최종 동작 모습**
# **Final action**

- Third terminal
  
```
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```

https://github.com/user-attachments/assets/be84e496-665a-4962-ac85-fcb81e43c1f2
