# Set up new Mac

### Terminal
ohmyzsh - https://github.com/robbyrussell/oh-my-zsh


### Android Studio
In OSX (Mac), the installations is very similar to Windows. First of all, download the JDK from Oracle website. The installation should occur fine, just follow the installation wizard.

Then, download Android Studio. The dmg file installation is very similar to any other installation of an OSX program, just drag and drop and you’re ok. When you execute it for the first time, it will download the needed SDKs and HAXM for better emulation.
The last step is to setup the environment variables, used for command line builds and tooling. Since you didn’t changed the default paths when installing, add the following to your ~/.bash_profile file (if the file doesn’t exist, create it).
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_111.jdk/Contents/Home
export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$JAVA_HOME/bin:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools


