# Test-Automation-with-Jenkins-and-RobotFramework
Locally independent test scripts. The configuration parameters are retrieved from the environment variables. Git hook auto trigger configured.

Added a git hook that triggers build automatically when a change is committed
Made all build/flash/test scripts installation independent. All local installation related settings are
retrieved from environment variables (MCUXpresso path, Robot Framework com-ports etc.)
Added the required environment variables to the Node setting to make sure that all executed scripts 
are stored in the repository. 
Robot framework plugin to see the test status.

### The config files for MCU_xpresso is not attached here. 
