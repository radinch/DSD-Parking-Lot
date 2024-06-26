# Final-compensation-Q8
This Verilog project simulates a parking control circuit for a university. Space of this parking have been divided to two different parts. One part for university staff and another for free cars. Capacity of these spaces changes with respect to hours of day. This circuit provides proper outputs for identifying state of the parking in each time of the day.

![_image.jpg](https://github.com/radinch/Final-compensation-Q8/blob/main/image.jpg)

## Tools
- Verilog
- ModelSim

## Implementation Details
We can divide our process to these steps:
- Designing Parking module
- Designing TB module

  
## Parking module
In this module we get some input signals that determine an entrance or exit of a car. With respect to this signals we provide some outputs that specify state of the parking. Now we explain module ports. For finding more details you can refer to the Documentation file.
### Inputs
- current_time : 5 bit wire ranges from 0 to 23 that shows hour of the day.
- car_entered: determines weather a car entered or not.
- is_uni_car_entered: determines weather entrance car belongs to university staff or not.
- car_exited: determines weather a car exited or not.
- is_uni_car_exited: determines weather exit car belongs to university staff or not.

### Outputs
- uni_vacated_space: remained capacity for university staff.
- vacated_space: remained capacity for non-staff.
- uni_parked_car: number of parked cars that belong university staff.
- parked_car: number of parked cars that don't belong university staff.
- uni_is_vacated_space: determines weather free space exists for staff.
- is_vacated_space: determines weather free space exists for non-staff.

## TB module
For testing this circuit after defining test bench file and it's inputs and outputs and simulating time, first of all we push 400 cars to testing parking more properly.
Then we wrote a python code to generate random testcases for this circuit. You can see this py file in code zip. Also you can see tempalate of our testcases in Documentation file. For better comperhension we recommend you to investigate TB module in code zip.
## Authors
- [Radin Cheraghi](https://github.com/radinch)


