# 제어 2팀 simulation_project

## (우분투 사용자)

1. rosdep install --from-paths src --ignore-src -r -y

## (민트 사용자)

2. rosdep install --from-paths src --ignore-src -r -y --os=ubuntu:focal

## catkin_make 에러 발생 시 설치 한 것들
1) sudo apt install ros-melodic-pid
2) sudo apt install ros-melodic-joy
3) sudo apt install ros-melodic-amcl
4) sudo apt install ros-melodic-map-server
5) sudo apt install ros-melodic-move-base
6) sudo apt install ros-melodic-gazebo-plugins

## Gazebo 맵이 정상적으로 안 뜰때 
https://github.com/osrf/gazebo_models 다운 후 ./gazebo/models에 복사

## URI 태그는 절대경로만 가능해서 각 PC 마다 변경해야 한다.

## 초기 launch 실행 방법
 1) roslaunch final_project costa_launch.launch            #costa카페 월드 열기
 2) roslaunch final_project put_robot_in_world.launch      #지정된 위치로 로봇 배치
 3) roslaunch final_project gmapping.launch                #mapping node  (*이미 맵을 만들었으니 사용할일 x)
 4) roslaunch final_project amcl.launch                    #localization node 
 5) roslaunch final_project navigation.launch              #전체 navigation 진행. (path planning 담당분이 여기에 추가해주시면 됩니다)

 




