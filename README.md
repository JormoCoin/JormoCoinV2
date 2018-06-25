![image](https://i.imgur.com/SKG6YnP.jpg)

When I look at most modern altcoins I see amazing and unique ideas. The thing is that's what they are "ideas". They make plans and goals they can't or won't achieve. The greediness for money is driving scams all over internet. I am seeing more and more cryptocurrencies release as time goes on but mining seems to be getting left behind. When I go into the communication platforms used by many cryptocurrencies I see aggressive behavior creating an unsafe or unproductive environment. All of these are driving the altcoin community down a dark path. With Jormo I want to lead the altcoin community down a better more productive path. Jormo is a coin that thrives to stay with miners and community in mind. We will not have an ICO and instead bring people back together to mine. This does not mean you can't buy Jormo it just means you will have to wait until it gets on an exchange.

To really learn more about Jormo I encourage you to read the whitepaper as I want to save space on this website to be a hub of links and basic info. View the whitepaper here.

To start mining download the cli under releases, create a wallet, and connect to a pool (See List Below). We also have a GUI wallet available here: https://github.com/JormoCoin/GUIWallet/releases.

Need help? Join the discord https://discord.gg/4ZA8dRY/.

### List Of Pools

- https://pool.jormo.org/
- https://getpool.org/jor/
- https://npool.pw/jor/
- http://jor.wahaobi.com/

Want your pool added? Message 1crusher in the discord.

### How To Compile

#### Linux

##### Prerequisites

- You will need the following packages: boost (1.55 or higher), rocksdb, cmake, git, gcc (4.9 or higher), g++ (4.9 or higher), make, and python. Most of these should already be installed on your system.
- For example on Ubuntu: `sudo apt-get install -y build-essential python-dev gcc g++ git cmake libboost-all-dev librocksdb-dev`
- If you are using Ubuntu and your version of Ubuntu doesn't have librocksdb-dev, you can get it from a ppa instead:
```
sudo add-apt-repository ppa:ethcore/ethcore -y
sudo apt-get update
sudo apt-get install librocksdb-dev
```

##### Building

- `git clone https://github.com/JormoCoin/JormoCoinV2`
- `cd jormocoin`
- `mkdir build && cd $_`
- `cmake ..`
- `make`

#### Apple

##### Prerequisites

- Install [cmake](https://cmake.org/). See [here](https://stackoverflow.com/questions/23849962/cmake-installer-for-mac-fails-to-create-usr-bin-symlinks) if you are unable call `cmake` from the terminal after installing.
- Install the [boost](http://www.boost.org/) libraries. Either compile boost manually or run `brew install boost`.
- Install XCode and Developer Tools.

##### Building

- `git clone https://github.com/JormoCoin/JormoCoinV2`
- `cd jormocoin`
- `mkdir build && cd $_`
- `cmake ..` or `cmake -DBOOST_ROOT=<path_to_boost_install> ..` when building
  from a specific boost install. If you used brew to install boost, your path is most likely `/usr/local/include/boost.`
- `make`

The binaries will be in `./src` after compilation is complete.

Run `./src/jormocoind` to connect to the network and let it sync (it may take a while).

#### Windows 10

##### Prerequisites
- Install [Visual Studio 2017 Community Edition](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15&page=inlineinstall)
- When installing Visual Studio, it is **required** that you install **Desktop development with C++** and the **VC++ v140 toolchain** when selecting features. The option to install the v140 toolchain can be found by expanding the "Desktop development with C++" node on the right. You will need this for the project to build correctly.
- Install [Boost 1.59.0](https://sourceforge.net/projects/boost/files/boost-binaries/1.59.0/), ensuring you download the installer for MSVC 14.

##### Building

- From the start menu, open 'x64 Native Tools Command Prompt for vs2017'.
- `cd <your_jormocoin_directory>`
- `mkdir build`
- `cd build`
- Set the PATH variable for cmake: ie. `set PATH="C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\IDE\CommonExtensions\Microsoft\CMake\CMake\bin";%PATH%`
- `cmake -G "Visual Studio 14 Win64" .. -DBOOST_ROOT=C:/local/boost_1_59_0` (Or your boost installed dir.)
- `MSBuild JormoCoin.sln /p:Configuration=Release /m`
- If all went well, it will complete successfully, and you will find all your binaries in the '..\build\src\Release' directory.
- Additionally, a `.sln` file will have been created in the `build` directory. If you wish to open the project in Visual Studio with this, you can.

#### Thanks
Cryptonote Developers, Bytecoin Developers, Monero Developers, Forknote Project, TurtleCoin Community, JormoCoin Developers

```
// Copyright (c) 2012-2017, The CryptoNote developers, The Bytecoin developers
// Copyright (c) 2014-2018, The Monero Project
// Copyright (c) 2018, The TurtleCoin Developers
// Copyright (c) 2018, The JormoCoin Developers
// 
// Please see the included LICENSE file for more information.
```
