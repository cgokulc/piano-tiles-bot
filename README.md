# Piano Tiles Bot

![Video](https://github.com/cgokulc/piano-tiles-bot/blob/main/pianotiles_bot.gif)

Game bot test on: https://www.silvergames.com/en/piano-tiles-2

### Working
- take a screenshot of rectangle with narrow width in the bottom tiles
- choose four points at the center of 4 bottom tiles and check its color 
- if the bolor is black, click that point
- loop over aboove steps

#### Note: Failsafe is mandotary
The inbuilt failsafe of pyautogui is to move mouse to upper-left point of the screen. In this example the program, the mouse is moved 10+ times every second, it may be impossible to move it to upper-left. So I included a failsafe of pressing 'q' to break the infinite loop using keyboard library. The last one want is to shut-down the laptop 'cause it click randomly.

### Improvements
- Every time a rectangular array of pixels are captured to just check color of 4 pixels. This can be optimised for improving samples per second.
- Alogorithms to check if the clicked tile has disappeared to avoid multiple clicks on same tile can be made
- A floating GUI to START/STOP bot can be made. 
