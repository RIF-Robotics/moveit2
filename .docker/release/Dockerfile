# moveit/moveit2:foxy-release
# Full debian-based install of MoveIt using apt-get

FROM ros:foxy-ros-base-focal
MAINTAINER Dave Coleman dave@picknik.ai

# Commands are combined in single RUN statement with "apt/lists" folder removal to reduce image size
RUN apt-get update && \
    apt-get install -y ros-${ROS_DISTRO}-moveit-* && \
    rm -rf /var/lib/apt/lists/*
