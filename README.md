# Scan Matching Localization

Self-Driving Car Engineer Nanodegree<br/>
https://www.udacity.com/course/self-driving-car-engineer-nanodegree--nd013

# Installation

Go to the Udacity workspace of the project "Scan Matching Localization" of the Lesson 3 "Localization" of the Self-Driving Car Engineer Nanodegree. Optionally, you can click on "Menu => Refresh Workspace..." if you want to get a fresh copy of the project.

Copy the contents of the file [c3-main.cpp](c3-main.cpp) into the file `/home/workspace/c3-project/c3-main.cpp` in the Udacity workspace of the project "Scan Matching Localization". You can do it by copying and pasting the contents of the file [c3-main.cpp](c3-main.cpp).

# Usage

Enable GPU Mode. Press the blue button "Desktop". Start one terminal in Desktop. Run the Carla simulator by using these Unix commands:

```
su - student # Ignore Permission Denied, if you see student@ you are good
cd /home/workspace/c3-project
./run_carla.sh
```

Start another terminal in Desktop. Compile the project by using these Unix commands:

```
cd /home/workspace/c3-project
cmake .
make
```

Run the project with the NDT algorithm by using Unix command:

```
./cloud_loc
```

Or run the project with the ICP algorithm by using Unix command:

```
./cloud_loc 2
```

Once the project is running, click on the map and tap the UP key 3 times. This improved version of the project normally works at the first run. However, if the green car gets left behind, run the project again and tap the UP key 3 times again.

The NDT algorithm works better than the ICP algorithm. Even if the car hits the wall at the end, the NDT algorithm will not produce an error greater than 1.2 meters.
# NDT image
![NDT](https://user-images.githubusercontent.com/22205974/156472384-abcd118f-b385-4ad0-b8fe-85aba8e92028.png)
![NDTimage](https://user-images.githubusercontent.com/22205974/156472388-aa44b95b-e786-4d2c-bb39-1a4e48d31b87.png)


# ICP image
![ICPimage](https://user-images.githubusercontent.com/22205974/156472409-4ce7955b-0e16-41a7-9b4e-afd6d6b3ae53.png)

