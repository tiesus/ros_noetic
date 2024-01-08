FROM althack/ros:noetic-gazebo

# ** [Optional] Uncomment this section to install additional packages. **
#
# ENV DEBIAN_FRONTEND=noninteractive
# RUN apt-get update \
#    && apt-get -y install --no-install-recommends <your-package-list-here> \
#    #
#    # Clean up
#    && apt-get autoremove -y \
#    && apt-get clean -y \
#    && rm -rf /var/lib/apt/lists/*
# ENV DEBIAN_FRONTEND=dialog

# Set up auto-source of workspace for ros user
ARG WORKSPACE
RUN echo "if [ -f /opt/ros/noetic/setup.bash ]; then source /opt/ros/noetic/setup.bash; fi" >> /home/ros/.bashrc \
    && echo "if [ -f /workspaces/noetic_dev/devel/setup.bash ]; then source /workspaces/noetic_dev/devel/setup.bash; fi" >> /home/ros/.bashrc
