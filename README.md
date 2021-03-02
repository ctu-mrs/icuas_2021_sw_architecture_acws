# A  Multi-Layered  Software  Architecture  for  Aerial  CognitiveMulti-Robot  Systems  in  Power  Line  Inspection  Tasks

## System requirements
Required OS is Ubuntu 18.04 64-bit or their flavors that can install ROS Melodic. The suggested variant of OS installation is dual boot instead of virtualization that can be slow and can not handle well the simulation GUI. We use Gitman to manage the repository submodules. The repository are supposed to be compiled by catkin tools.

## Installation
  1. Follow the insctructions on the [MRS UAV System](https://github.com/ctu-mrs/mrs_uav_system) to install the MRS System. **After the installation please checkout the `uav_core` package to `icuas_2021_sw_architecture_acws` branch and rebuild the ROS workspace again**.
  2. Clone and build the [Aerial-Core](https://github.com/ctu-mrs/aerialcore_simulation/tree/icuas_2021_sw_architecture_acws) package. **Make sure to install the package on the `icuas_2021_sw_architecture_acws` branch**.
```bash
    cd ~\workspace\src\
    git clone git@github.com:ctu-mrs/aerialcore_simulation.git
    cd aerialcore_simulation
    git icuas_2021_sw_architecture_acws
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
