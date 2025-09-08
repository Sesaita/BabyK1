Work in Progress <br>
Inertia Toolhead Adaption for K1 8 or 10mm Y rods. (8mm are stock on k1)<br>

Travel will be roughly x 225 y 225 and <br>
Print Area roughly x 225 y 220 (The nozzle will go 5mm over the build plate to the front)<br>
##################################################################################<br>

Inertia Extruder<br>
Check their GitHub for the files, a bom is in their discord aswell.<br>
https://github.com/Inertia-Bros/Inertia-Cube<br>
(STLS -> Production Frame Build -> Monolithic Gantry -> Inertia Extruder)<br>

Inertia Mainbodies<br>
At the Moment only the Dragon ACE Volcano UHF is compatible.(Thats what im using)<br>
I can adjust for another/different Carriage/Mainbodie just message me or do it yourself :). <br>
https://github.com/Inertia-Bros/Inertia-Toolhead<br>
##################################################################################<br>

1x Inertia Toolhead Carriage modified for belt clips and nozzle lowered<br>
8x m3 voron heat insert(M3x5x4)<br>
4x m3x16 SHCS<br>
2x m3x6 flat head screws for carto/probe<br>

BCJ XY Joints<br>
4x m3 thin square nut<br>
2x m3 voron heat insert(M3x5x4)<br>
2x m3xXX BHCS<br>

1x BTT EBB36 Mount<br>
1x Inertia Extruder (Inertia Github)<br>
1x Inertia Mainbodie (Inertia Toolhead Github)<br>
##################################################################################<br>

Printer.cfg config <br>

[stepper_x]<br>
position_endstop: 225<br>
position_max: 225<br>

[stepper_y]<br>
position_endstop: 225<br>
position_max: 225 <br>

[BTTEBB36]<br>
[extruder]<br>
step_pin: BTTEBB36:PD0<br>
dir_pin: BTTEBB36:PD1<br>
enable_pin: !BTTEBB36:PD2<br>
microsteps: 16<br>
gear_ratio: 9:1<br>
rotation_distance: 35.1805<br>
nozzle_diameter: 0.4<br>
filament_diameter: 1.75<br>
heater_pin: BTTEBB36:PB13<br>
#sensor_pin: BTTEBB36:PA   # If connecting your hotend thermistor to TH0 on the toolhead MCU<br>
#sensor_type: PT1000<br>
#pullup_resistor: 2200<br>
pressure_advance_smooth_time: 0.020<br>
#control: pid<br>
#pid_Kp: 22.2<br>
#pid_Ki: 1.08<br>
#pid_Kd: 114<br>
min_temp: 0<br>
max_temp: 350<br>
min_extrude_temp: 10<br>
pwm_cycle_time: 0.01667<br>
max_extrude_only_distance: 1000.0<br>
max_extrude_cross_section: 80<br>
sensor_type: MAX31865<br>
sensor_pin: BTTEBB36: PA4<br>
spi_bus: spi1<br>
rtd_nominal_r: 430<br>
rtd_nuim_of_wires: 2<br>

[tmc2209 extruder]<br>
uart_pin: BTTEBB36:PA15<br>
run_current: 0.6<br>
sense_resistor:0.110<br>
##################################################################################<br>

![K1 Inertia Toolhead](https://github.com/Sesaita/BabyK1/blob/main/WIP%20Inertia%20Toolhead%20K1/K1%20Inertia%20Toolhead%201.jpg) 
![K1 Inertia Toolhead](https://github.com/Sesaita/BabyK1/blob/main/WIP%20Inertia%20Toolhead%20K1/K1%20Inertia%20Toolhead%202.jpg) 
![K1 Inertia Toolhead](https://github.com/Sesaita/BabyK1/blob/main/WIP%20Inertia%20Toolhead%20K1/K1%20Inertia%20Toolhead%203.jpg) 
