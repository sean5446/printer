# printer
Creality Ender 3 v2 printer formware config

Modified to use Jyers, UBL, and Slice Engineerings 300*C Thermistor

Some changes from https://www.mironv.com/2020/08/14/ender3v2-bltouch-marlin/

```C
#define FAN_SOFT_PWM

#define X_DRIVER_TYPE TMC2208_STANDALONE
#define Y_DRIVER_TYPE TMC2208_STANDALONE
#define Z_DRIVER_TYPE TMC2208_STANDALONE

#define HOST_ACTION_COMMANDS
#if ENABLED(HOST_ACTION_COMMANDS)
  //#define HOST_PAUSE_M76
  #define HOST_PROMPT_SUPPORT
  //#define HOST_START_MENU_ITEM  // Add a menu item that tells the host to start
#endif

#define TEMP_SENSOR_0 5

#define HEATER_0_MAXTEMP 300
```
