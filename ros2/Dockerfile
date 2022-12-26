FROM osrf/ros:galactic-desktop

ENV SHELL /bin/bash

RUN apt-get update && apt-get install -y \
    vim \
    screen \
    git

RUN apt-get update && apt-get install -y \
    ros-galactic-turtlebot3 \
    ros-galactic-turtlebot3-simulations

RUN echo "source /opt/ros/galactic/setup.bash" >> ~/.bashrc \
    && /bin/bash -c "source ~/.bashrc"

RUN apt-get update && apt-get install -y \
    ros-galactic-rosbridge-suite

ENV TURTLEBOT3_MODEL waffle