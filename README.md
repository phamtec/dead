# dead

Dictionary Editor's Aren't Dead

A Dictionary editor using SDL.

## Prerequsists

#### Linux

```
sudo apt-get install -y git g++ gcc build-essential git make \
  pkg-config cmake ninja-build gnome-desktop-testing libasound2-dev libpulse-dev \
  libaudio-dev libjack-dev libsndio-dev libx11-dev libxext-dev \
  libxrandr-dev libxcursor-dev libxfixes-dev libxi-dev libxss-dev libxtst-dev \
  libxkbcommon-dev libdrm-dev libgbm-dev libgl1-mesa-dev libgles2-mesa-dev \
  libegl1-mesa-dev libdbus-1-dev libibus-1.0-dev libudev-dev libpipewire-0.3-dev \
  libwayland-dev libdecor-0-dev liburing-dev libfreetype-dev
```

### Boost

#### Linux

```
wget https://github.com/boostorg/boost/releases/download/boost-1.85.0/boost-1.85.0-b2-nodocs.tar.gz
tar xzf boost-1.85.0-b2-nodocs.tar.gz 
cd boost-1.85.0
./bootstrap.sh --prefix=/usr
sudo ./b2 install boost.stacktrace.from_exception=off
```

#### Mac

```
brew install boost@1.85.0
```

### SDL

#### Mac

```
brew install sdl3
```

#### Linux

```
git clone https://github.com/libsdl-org/SDL
cd SDL
mkdir build
cd build
cmake ..
make
sudo make install
```

### SDL TTF support

#### Mac

```
brew install sdl3_ttf
```

#### Linux

```
git clone https://github.com/libsdl-org/SDL_ttf
cd SDL_ttf
mkdir build
cd build
cmake ..
make
sudo make install
```

## Building this project

```
mkdir build
cd build
cmake ..
make
```

## Running this

```
$ ./dead
```

Hit q to exit

## Progress

Draws a spinning hello world using opengl.

## Current Focus

Layout a simple dictionary using SDL in a nice TTF font.

## Change Log

### 25-Jul-2025

Hello world. First checkin.

