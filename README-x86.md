# Standalone compiling the pub/sub clients 
g++ --std=c++17 -c -o main.o main.cpp
g++ --std=c++17 -c -o procfs.o procfs.cpp
g++ --std=c++17 -c -o utils.o utils.cpp
g++ --std=c++17 -c -o json_manager.o json_manager.cpp
g++ --std=c++17 -c -o MQTTManager.o MQTTManager.cpp
gcc -c -o lib/cJSON.o lib/cJSON.c
g++ --std=c++17 -o myNewApp main.o procfs.o utils.o json_manager.o lib/cJSON.o MQTTManager.o -L./lib ./lib/libmosquitto.so.1  -Wl,-rpath=./lib

