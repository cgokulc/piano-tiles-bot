# Piano Tiles Bot

![Video](https://github.com/cgokulc/piano-tiles-bot/blob/main/pianotiles_bot.gif)

I tested this game bot on: https://www.silvergames.com/en/piano-tiles-2

### Working
- take a screenshot of rectangle with narrow width in the bottom tiles
- choose four points at the center of 4 bottom tiles and check its color 
- if the bolor is black, click that point
- loop over aboove steps

#### Note: Failsafe in mandotary
The inbuilt failsafe of pyautogui is to move mouse to upper-left point of the screen. In this example the program, the mouse is moved 10+ times every second, it may be impossible to move it to upper-left. So I included a failsafe of pressing 'q' to break the infinite loop using keyboard library. The last one want is to shut-down the laptop 'cause it click randomly.
