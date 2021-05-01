A demo Arduino sketch for the [WT32-SC01](https://www.seeedstudio.com/ESP32-Development-board-WT32-SC01-p-4735.html).

To install:

1. Clone this repo.
2. Set up your Arduino IDE with ESP32 support.
3. In your Arduino libraries directory, clone [a fork of Adafruit_FT6206_Library](https://github.com/sowbug/Adafruit_FT6206_Library) that allows overriding the I2C GPIO pins in the Arduino Wire library.
4. Add TFT_eSPI via Arduino's library manager.
5. Configure TFT_eSPI by copying `WT32-SC01-User_Setup.h` from this directory to wherever you keep your TFT_eSPI user setup files (read that project's documentation to see how to do that), and then point TFT_eSPI to that header file.

Now build and flash to your device. If everything goes well, you'll see a rotating cube on the screen, and when you tap the screen, the background will alternate between black and green.

Thanks to [seaniefs](https://github.com/seaniefs/WT32-SC01-Exp) for getting me started. This project is basically a redo of that project, but updated for a newer version of the Adafruit touchscreen library.
