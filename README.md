# SPIKE Prime API
## Info
This is a simpler and more intuitive API which runs on SPIKE 3. Just fork this repo and put your main.py in the official lego SPIKE Prime 3 editor. Add your code at the end of the port after the comment. You may remove the comment if you wish.
## Documentation
If something is all capitalized e.g. "ABCD" it is to be replaced. If something is "?" followed by all capitalized e.g. "?ABCD" it is optional and can be replaced. If two optional arguments are excluded, ", , " is implicitly converted to ", ".
If LEFT_SPEED is changed, LEFT_SPEED's default will be edited. Same with right_speed. If speed is changed, left_speed and right_speed will be changed. The default speed will be 100 if never changed. The default wheel diameter will be 88.
| Word Block | Python
|---|--|
| ![move_forward_for_rotations](./images/move_forward_for_rotations.png) | ```move.forward_for(ROTATIONS, "rotations", ?LEFT_SPEED, ?RIGHT_SPEED)```|
| ![move_forward_for_degrees](./images/move_forward_for_degrees.png) | ```move.forward_for(DEGREES, "degrees", ?LEFT_SPEED, ?RIGHT_SPEED)```|
| ![move_forward_for_seconds](./images/move_forward_for_seconds.png) | ```move.forward_for(SECONDS, "seconds", ?LEFT_SPEED, ?RIGHT_SPEED)```|
