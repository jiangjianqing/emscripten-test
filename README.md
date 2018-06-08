##注意
### Fetch the latest registry of available tools.
./emsdk update

### Download and install the latest SDK tools.
./emsdk install latest

###Make the "latest" SDK "active" for the current user. (writes ~/.emscripten file)
./emsdk activate latest

### Activate PATH and other environment variables in the current terminal
source ./emsdk_env.sh

###在用户目录下，存在.emscripten_xxx等目录，在第一次用emcc命令进行编译时，会将stdio.h等c标准库编译成中间代码存放在.emscripten_cache中，以提高后续编译的速度.

##环境准备
每次使用emcc都需要执行如下命令：
source ./emsdk_env.sh

##执行编译
emcc hello_world.c
