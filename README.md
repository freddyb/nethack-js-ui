# User Interface for [nethack-3.4.3-js](https://github.com/freddyb/nethack-3.4.3-js)



This repository hosts the user interface (experiments) for my port of nethack-3.4.3 to the web.

For more information, check out [nethack-3.4.3-js](https://github.com/freddyb/nethack-3.4.3-js).



### UI Details
The user interface aims to replicate the ones used in the Android and iOS ports, namely a set of pre-defined buttons for the most used commands (search, wait, read, throw, zap wand, ..) and two extra buttons for extended commands (e.g., ` #loot`) and showing a keyboard.

### The keyboard hack
We can not trigger whether a keyboard is shown or not on a mobile web page. To achieve this we trigger focus/blur events on an invisible `<input>` element and then redirect key events on this element to the game.