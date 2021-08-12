# This is an auto generated Dockerfile for ros:ros-core
# generated from docker_images/create_ros_core_image.Dockerfile.em
FROM ros:noetic
ENV ROS_DISTRO noetic

# copy example files
COPY catkin_ws /catkin_ws
WORKDIR /catkin_ws/
RUN . /opt/ros/noetic/setup.sh && catkin_make

# setup entrypoint
COPY ./ros_entrypoint.sh /
ENTRYPOINT ["/ros_entrypoint.sh"]



CMD ["bash"]