# SPIKE Prime API
## Info
This is a simpler and more intuitive API which runs on SPIKE 3. Just fork this repo and put your main.py in the official lego SPIKE Prime 3 editor. Add your code at the end of the API after the comment. You may remove the comment if you wish.
## Documentation
### Simple example
![python and word blocks side by side](./images/python_wordblock_side_by_side.png)
### Movement
#### General info
If something is all capitalized e.g. "ABCD" it is to be replaced. If something is "?" followed by all capitalized e.g. "?ABCD" it is optional and can be replaced. If two optional arguments are excluded, ", , " is implicitly converted to ", ".
If LEFT_SPEED is changed, LEFT_SPEED's default will be edited. Same with right_speed. If speed is changed, left_speed and right_speed will be changed. The default speed will be 100 if never changed. The default wheel diameter will be 88.
#### Word Block to Python Conversion Table 
| Word Block | Python | Notes
|---|---|---|
| ![move forward for rotations](./images/move_forward_for_rotations.png) | ```move.forward_for(ROTATIONS, "rotations", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves forward for ROTATIONS rotations at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move forward for degrees](./images/move_forward_for_degrees.png) | ```move.forward_for(DEGREES, "degrees", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves forward for DEGREES degrees at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move forward for seconds](./images/move_forward_for_seconds.png) | ```move.forward_for(SECONDS, "seconds", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves forward for SECONDS seconds at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move forward for cm](./images/move_forward_for_cm.png) | ```move.forward_for(CM, "cm", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves forward for CM cm at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move forward for in](./images/move_forward_for_in.png) | ```move.forward_for(IN, "in", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves forward for IN in at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move backward for rotations](./images/move_backward_for_rotations.png) | ```move.backward_for(ROTATIONS, "rotations", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves backward for ROTATIONS rotations at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move backward for degrees](./images/move_backward_for_degrees.png) | ```move.backward_for(DEGREES, "degrees", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves backward for DEGREES degrees at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move backward for seconds](./images/move_backward_for_seconds.png) | ```move.backward_for(SECONDS, "seconds", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves backward for SECONDS seconds at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move backward for cm](./images/move_backward_for_cm.png) | ```move.backward_for(CM, "cm", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves backward for CM cm at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![move backward for in](./images/move_backward_for_in.png) | ```move.backward_for(IN, "in", ?LEFT_SPEED, ?RIGHT_SPEED)```|Moves backward for IN in at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![start moving forward](./images/start_moving_forward.png) | ```move.forward(?LEFT_SPEED, ?RIGHT_SPEED)```|Moves forward until direction to stop at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![start moving backward](./images/start_moving_backward.png) | ```move.backward(?LEFT_SPEED, ?RIGHT_SPEED)```|Moves backward until direction to stop at LEFT_SPEED speed for the left wheel and RIGHT_SPEED speed for the right wheel
| ![set movement speed to](./images/set_movement_speed_to.png) | ```move.set_speed(SPEED)```|Sets default speed to SPEED as above in general info
| ![set movement motors to](./images/set_movement_motors_to.png) | ```move=MotorPair(LEFT_PORT, RIGHT_PORT, ?WHEEL_DIAMETER_MM, ?ONE_MOTOR_ROTATION_IN_CM)```|Sets movement motors. Also needs either WHEEL_DIAMETER_MM or ONE_MOTOR_ROTATION_IN_CM must be passed. Both must not be passed.
| ![set 1 motor rotation_cm](./images/set_1_motor_rotation_cm.png) | ```move.set_motor_rotation(ONE_MOTOR_ROTATION_IN_CM)```|Sets distance moved in cm by one motor rotation.
