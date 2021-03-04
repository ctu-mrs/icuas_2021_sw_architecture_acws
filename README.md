# A  Multi-Layer Software Architecture for Aerial Cognitive Multi-Robot Systems in Power Line Inspection Tasks

## System requirements
Required OS is Ubuntu 18.04 64-bit or their flavors that can install ROS Melodic. The suggested variant of OS installation is dual boot instead of virtualization that can be slow and can not handle well the simulation GUI. We use Gitman to manage the repository submodules. The repository are supposed to be compiled by catkin tools.

## Installation
  1. Follow the insctructions in the [MRS UAV System](https://github.com/ctu-mrs/mrs_uav_system#installation) repository to install the MRS System.
  2. After the installation checkout the `uav_core` package to `icuas_2021_sw_architecture_acws` branch and rebuild the `mrs_workspace` again.
```bash
    cd ~/mrs_workspace/src/uav_core/
    git checkout icuas_2021_sw_architecture_acws
    catkin build
```
  2. Clone and build the [Aerial-Core](https://github.com/ctu-mrs/aerialcore_simulation/tree/icuas_2021_sw_architecture_acws) package.
```bash
    cd ~/workspace/src/
    git clone git@github.com:ctu-mrs/aerialcore_simulation.git
    cd aerialcore_simulation
    git checkout icuas_2021_sw_architecture_acws
    catkin build
```
  3. Clone and build the [Trajectory loader](https://github.com/ctu-mrs/trajectory_loader/tree/icuas_2021_sw_architecture_acws) package.
```bash
    cd ~/workspace/src/
    git clone git@github.com:ctu-mrs/trajectory_loader.git
    cd trajectory_loader
    git checkout icuas_2021_sw_architecture_acws
    catkin build
```

## Running the simulation
### Inspection
  1. Go to ```scripts\inspection\``` folder and launch ```start.sh```
```bash
cd scripts\inspection\
./start.sh
```
### Safety
  1. Go to ```scripts\safety\``` folder and launch ```start.sh```
```bash
cd scripts\safety\
./start.sh
```
## Multimedia materials
Additional information and multimedia material are reported [on the website](http://mrs.felk.cvut.cz/software-architecture-acws). More about the project can be found on the [MRS website](http://mrs.felk.cvut.cz/projects/aerial-core). 

[![Safety scenario](https://github.com/ctu-mrs/icuas_2021_sw_architecture_acws/wiki/imgages/main.png)](https://youtu.be/c6_GIUFoGhU "Gazebo simulations")
