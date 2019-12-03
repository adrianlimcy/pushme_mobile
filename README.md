Troubleshooting

https://stackoverflow.com/questions/26483370/android-emulator-error-message-panic-missing-emulator-engine-program-for-x86/49511666#49511666

Step 1: In my case the order was important, first emulator and then tools.

export ANDROID_SDK=$HOME/Library/Android/sdk
export PATH=$ANDROID_SDK/emulator:$ANDROID_SDK/tools:$PATH
Step 2: Reload you .bash_profile Or .bashrc depending on OS

Step 3: Get list of emulators available: $emulator -list-avds

Step 4: Launch emulator from the command line and Replace avd with the name of your emulator $emulator @avd

Just step 1 and 2 will do usually

How to reload the bash_profile?
1. Simply type source ~/.bash_profile
2. Alternatively, if you like saving keystrokes you can type . ~/.bash_profile
