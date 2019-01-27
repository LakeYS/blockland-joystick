# Development Notice
I currently do not have plans to further develop this project, however you are free to fork it for your own uses. I have included some of my personal notes and documentation below for reference.


# blockland-joystick
This is a project that aims to expand Blockland's controller ("joystick") support as much as possible using only Torque code. It even has partial support for menu navigation by moving the mouse.

# Features
- Play the game entirely with a controller!
- Build with a controller. When the brick box is up, the controller is in build mode.
- GUI support (WIP)

# Controls
***Main Controls***

- RT - Mouse Fire
- LT - Toggle Build Controls
- LB - Jet
- RB - Toggle Tool Box
- A - Jump
- B - Crouch
- X - Light
- Y - Switch First/Third Person
- Start - Escape
- Select/Back - Toggle Alt Controls
- D-Pad Up - Scroll Inventory Up (Opens Tools)
- D-Pad Down - Scroll Inventory Down (Opens Tools)
- D-Pad Left - Scroll Inventory Left (Opens Paint)
- D-Pad Right - Scroll Inventory Right (Opens Paint)
- (D-Pad only scrolls specified box if it is already open)

- Press Left Stick - Bricks Menu
- Press Right Stick - Chat Menu

(Toggling build controls is set to the left trigger (instead of the bumper) because only one trigger can be used at a time)

***Build Mode Controls***

(Can still walk, crouch, jet, and use bricks/chat; cannot look; the brick box is always up when this is on)
- LT - Open Brick Bar (Toggles build mode)
- RB - Scroll Inventory Right (Bricks Bar; Hold to quick scroll)
- RT - Plant Brick
- A - Mouse Fire
- B - Undo Brick
- X - Rotate Brick
- Y - Toggle Super Shift (Toggle? hopefully this can be held too. check - this)
- Right Stick - Shift Brick

- D-Pad Up - Shift Brick Up 1/3
- D-Pad Down - Shift Brick Down 1/3
- D-Pad Left - Scroll Brick Bar Left
- D-Pad Right - Scroll Brick Bar Right

(The D-Pad is used for vertical shift instead of regular directions so the player can walk and shift forward at the same time)
(RT is used for brick planting so you can shift and plant at the same time. This is very useful at times.)

***Alt Controls***

(Toggle-able with select/back, disables super shift/vertical shift and/or build mode)
(Can still walk, look, crouch, and jet)
- Left Stick - Toggle Build Macro Recording
- Right Stick - Playback Build Macro
- A - Drop Camera at Player
- B - Drop Player at Camera
- X - Drop Tool
- Y - Toggle Player Names/Crosshair
- Hold LB - Emote Mode
- D-Pad Up - Scroll chat up
- D-Pad Down - Scroll chat down
- D-Pad Left - Previous Vehicle Seat
- D-Pad Right - Next Vehicle Seat

***Emote Mode***
- A - Love
- B - Hate
- X - Confusion
- Y - Alarm
- D-Pad Up - Zombie
- D-Pad Down - Sit

# To-Do
- Finish "simple" GUI support. Move the mouse and click things like normal.
- An options menu for the controller.
- In-game keyboard for chat (Possibly with a "daisy wheel" keyboard like the one in Steam's big picture mode)
- Misc. useful keybinds that aren't included already (Opening the server list and "start a game" GUIs, etc)\
- (Maybe) "Advanced" GUI navigation. You can scroll through buttons rather than moving a cursor.
- (Maybe) Controller keybinds
- Keybinds in chat, center print, and bottom prints. Example: Typing "[Jump]" in chat will show "Space" (or "A" for controllers).
- (Maybe) A "help" overlay. Shows a controller on-screen with labelled buttons.
- Steam controller integration?

# Snippets
## Return the top GUI element
```
canvas.getObject(canvas.getCount()-1);
button.setValue(1);
```

## bindCmd
http://docs.garagegames.com/torque-3d/reference/classActionMap.html#acff303d313ce4e08bcec9f468f6c26a5
