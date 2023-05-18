
Fork of https://github.com/moggieuk/ERCF-Software-V3
everything on the ERCF-Software-V3 "Happy Hare" is there

# State: tested and working
next iteration:
- cut length per Tool (0 = no cut)
- speed optimization


## NEW for users in comparison of ERCF-Software-V3 "Happy Hare" 30.04.2023  
ercf_parameters.cfg:  
cutter_enable: 0						# Cutter Disable = 0 , Enable = 1  
cutter_sensor_calibration_length: 200	# similar to calibration_bowden_length for the cutter sensor  
cutter_blade_sensor: 30.5 				# Distance of cutter sensor to blade  
cutter_offcut_length: 3   				# length of cutoff  
cutter_servo_down_angle: 90				  
cutter_servo_up_angle: 90				  
cutter_servo_duration: 0.2				# Duration of PWM burst sent to cutter servo (automatically turns off)  
cutter_homing_step: 1.0					# Stepsize of the cutter sensor homing  
cutter_homing_max: 25 					# Distance: search for cutter sensor  
cutter_stop_before_sensor: 5 			# Distance: how far from the sensor the fast move should stop  
  
ercf_hardware.cfg:  
CUTTER SERVO  
CUTTER SENSOR  

MACROS:  
ERCF_CALIBRATE_CUTTER_HOME				# Cutter Sensor Homing Distance Calibration  
ERCF_TEST_CUT							# Test cut of Tool = x (x default 0)  

