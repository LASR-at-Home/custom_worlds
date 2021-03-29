## Compatibility (please read if accessing from DEC-10)

master branch was updated to work with the downloadable container released for 2020.

For containers **built from source** via tiago-lib (DEC-10 included):

    git fetch
    git checkout 2019-version


## Instructions


To clone this specific branch:

    git clone --single-branch --branch wrs-2020_worlds https://gitlab.com/sensible-robots/custom_worlds.git

To setup the mappings:

    Outside of the container, `cd custom_worlds && ./setup.sh
    
To launch wrs2020 world:

    roslaunch custom_worlds wrs2020.launch

To launch custom_worlds in mapping mode:

    roslaunch custom_worlds tiago_mapping.launch world:="<world_name>"


to launch custom_worlds in navigation mode:

    roslaunch custom_worlds tiago_navigation.launch world:="<world_name>"


Please note that the `.world` suffix should be ommitted.

## Directories

- Worlds can be found in and added to the **/worlds** directory.
- 3D models can be found in and added to the **/models** directory.
- Quick-launch files for navigation can be found in the **/launch** directory.
