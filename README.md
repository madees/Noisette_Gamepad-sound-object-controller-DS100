# Noisette_Gamepad-sound-object-controller-DS100
Example file for Chataigne DS100 module, sound object remote with a gamepad.

A simple interface to act as as Soundscape sound object controller, as "side-car" for any FOH mixing, artists on stage etc.

## Tested with
Chataigne v1.9.24 and DS100 Module 2.4.1

## How to setup
1. Connect a gamepad (USB, bluetooth ... according to its manual).
2. Download the .noisette and its .js scripts and extract them in the same folder. (you may use the "<> Code" button, "Local" tab, "Download zip" above)
3. Launch Chataigne.
4. First install DS100 OSC module (in Chataigne/Files menu/Community module manager...).
5. Open the .noisette file
6. In Gamepad module Parameters, set the Device accordingly to your model.
7. In DS100 module OSC output setting, set the IP to control port of DS100 device.

## Features
It uses a standard Gamepad "360" type: 
![](https://github.com/madees/Noisette_Gamepad-sound-object-controller-DS100/blob/main/360_controller.png)

### Change controlled object index #
(see the Dashboard for feedback of index number, object name etc.)
- Left Bumper: Decrease Object index -1
- Right Bumper: Increase Object index +1

### Move object
- Left Stick: (SLOW RELATIVE MOTION) Move the object in the joystick direction. Speed of displacement can be control by the amount of deviation.
- Left Stick Button press: (RESET) Set object to center (0,0) position. 
- Left Stick + Button: (FAST DISPLACEMENT) Position the object to absolute joystick position.
- D-Pad: (FINE MOVE) Move the object precisely by fine steps. On Dashboard, you can set the amount of "fine step".

### En-Space reverb send
- Right Stick up/down: (REVERB) Increase or decrease the send level.
- Right Stick Button: (DRY) Mute send (toggle).

### Spread
- Right Stick left/right: (SPREAD) set the object spread.

### Temporary mute
- B Face Button: (CUT) Mute object when pressed.

### Circlizer
Those are giving more control to play with, by playing with azimuth animation and distance.
When you use it, the original object position (controlled by Left joystick/D-Pad) is now the center of a circle.
- Left Trigger: (DISTANCE) Radius of the circle (distance from center).
- Right Trigger: (SPEED) Rotation frequency
- Y Face Button: (CW/CCW) Direction of rotation
- X Face Button: (HOLD) If you press it, you can release the triggers and the parameters are kept. Pressing it again and object stop turning and return to center position, and you can use the Distance and Speed triggers again.
- A Face Button: (TAP) Tap tempo and reset (using Right Trigger will set the "phase" initial position). In "hold" of a Distance, you can adapt the Speed by taping a tempo.

### Pair
Couple a second object with the seleted one. It uses N+1 object. 
You have from now fours modes : Copy (same position for both objects), Mirror X only, Mirror Y only, Mirror X and Y.
- Start Button: (PAIR) De/activate pairing.
- Back Button: (MODE) Choose pairing mode. Press sequentially to go thru modes.


## More to come
Always modifying it, may upload variants...

For global support on how to use Chataigne and its modules, or this example project, please visit the forum : http://benjamin.kuperberg.fr/chataigne/forum or join us on Discord : https://discord.com/invite/ngnJ5z 

If you need any help, my contact on Discord is also "madees". Any feedback or ideas on improvements or features are welcome !
