# ROS 로봇을 부팅시부터 기동시키는 방법

ROS로 개발이 완료되고 나면 개발된 로봇을 최초 부팅시켰을 때 로봇을 자동으로 구동해야 한다.<br/>
이를 위해서 ROS에서는 robot_startup 패키지를 제공하고 있다.

* 저장소 : https://github.com/clearpathrobotics/robot_upstart

## 사용 방법
### 설치
rosrun robot_upstart install pkg/path

```
rosrun robot_upstart install turtlebot3_bringup/turtlebot3_robot.launch
```

옵션
```
[--user NAME]
[--setup path/to/setup.bash]
[--rosdistro DISTRO]
[--master http://MASTER:11311]
[--logdir path/to/logs]
[--augment]
[--provider [upstart|systemd]]
[--symlink]
pkg/path [pkg/path]
```

### 삭제
```
rosrun robot_upstart uninstall JOBNAME
```
옵션
```
[--rosdistro DISTRO]
JOBNAME
```