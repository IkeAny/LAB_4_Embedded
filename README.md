# LAB_4_Embedded
By: Ronan Harkins, Zachary Bravo, Ike-Anyanwu Chinedu
Introduction
The goal of lab for was to toggle the on board LED with a 250 ms delay and produce a duty cycle with the timer within the MSP430FR2355. With this the the ouput should be sent to a pin on the board and the values should be able to be seen on the oscilloscope within the lab.

10 Percent Duty Cycle
For the ten percent duty cycle the values of TB0CCR0 was changed to be 500 and the value of TB0CCR1 was change to a value of 50. The reason this value was changed to 50 was because of the way the duty cycle is set. In order to obtain a duty cycle of 10% a value of 0.1 was needed from the combination of TB0CCR1 divided by TB0CCR0. Since the values used within the code was 50/500 the output of this is 0.1 providing the correct duty cycle that is needed for part 1 of the lab. The duty cycle that was produced can be seen within the figure below.Within this figure it can be seen that a duty cycle of about ten can be seen. The reason it is not excat is beause of the wires that are being used are going to lose some of the signal. This process was done using the polling method.

![image](https://user-images.githubusercontent.com/75408516/202005706-505a3874-9247-470a-9670-a8e9a6248683.png)

![image](https://user-images.githubusercontent.com/75408516/202005792-ae2a14fa-2909-40a2-adfb-ca00f02c6dcf.png)


20 Percent Duty Cycle
For the 20% duty cycle the same method was applied however instead of using the polling method the interupt method was used. This does not change how the duty cycle is calculated. The values of TB0CCR0 and TB0CCR1 needed to create a value of 0.2 in order to get the 20% duty cycle. So the value of TB0CCR1 was keep at 50 and the value of TB0CCR0 was changed to 250. The reason for this change is becasue the value 0.2 is need so 50/250 produces the value of 0.2 needed for the 20% duty cycle. This duty cycle can be seen within the figure below. Within the figure below it can be seen that the duty cycle is again off by a small amount. This is again due to the wires being used.

![image](https://user-images.githubusercontent.com/75408516/202005987-91049b55-25d0-4dac-bb6f-d863cc9eba10.png)

