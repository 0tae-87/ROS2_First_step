# **ROS2_First_Step**
- Gazebo 상에서 camera 구현을 목표로 진행함
- 블로그를 참조해서 진행함 https://with-rl.tistory.com/
- 가장 많은 문제를 일으켰던 것은 이전에 다른 공부를 위해 설치해둔 패키지와 충돌하면서 Gazebo가 실행되지 않음
  ERROR : Exit code -6, 2 등등 나타남
- 또 다른 문제로 colcon build 시 --symlink-install을 하게 되는데 이렇게 하면 디렉토리 불러올 때 오류 발생했음
  -> 이는 그냥 colcon build로 해결 가능
- 블로그에 패키지 이름 오타 있음 (test -> tutorial)



# **Gazebo에서 카메라 구현에 성공한 모습**


![Image](https://github.com/user-attachments/assets/e4c83abd-4975-4013-8eb0-60d75e18748f)

# **추가적으로 rviz2도 실행하여 연동에 성공한 모습**
![Image](https://github.com/user-attachments/assets/617f15ea-d44a-465d-85ee-144c6356b654)

+동영상 따로 첨부
