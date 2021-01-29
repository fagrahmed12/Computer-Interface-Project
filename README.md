# Computer-Interface-Project
The aim of this project is to design a temperature controlled fan using microcontroller,
in which the fan is automatically turned ON or OFF according to the temperature. 
The LM35 temperature sensor will give continuous analog output corresponding to the temperature sensed by it.
This analog signal is given to the ADC, which converts the analog values to digital values.
In order to get the temperature from the sensed analog voltage, we need to perform some calculations in the programming for the microcontroller.
Once the calculations are done by the microcontroller according to the logic, the temperature is displayed on the GUI.
The microcontroller will continuously monitor the temperature.
If the temperature exceeds more than 50 deg Celsius (as per the code), the microcontroller will turn on the relay to start the fan.
If the temperature drops below 40 deg Celsius (as per the code).



Working
The aim of this project is to design a temperature controlled fan using 8051 microcontroller, in which the fan is automatically turned ON or OFF according to the temperature. 
The working of the project is explained here.
In this circuit, the LM35 temperature sensor will give continuous analog output corresponding to the temperature sensed by it.
This analog signal is given to the ADC, which converts the analog values to digital values.
The digital output of the ADC is equivalent to sensed analog voltage.
In order to get the temperature from the sensed analog voltage, we need to perform some calculations in the programming for the microcontroller.
Once the calculations are done by the microcontroller according to the logic, the temperature is displayed on the LCD.
Like this, the microcontroller will continuously monitor the temperature.
If the temperature exceeds more than 50 deg Celsius (as per the code), 
the microcontroller will turn on the relay to start the fan. If the temperature drops below 40 deg Celsius (as per the code).




How Temperature Controlled DC Fan Circuit using Microcontroller Works?
1-Initially switch the power supply.
2-Microcontroller starts reading the temperature of the surroundings.
3-The analog value of temperature is given by the temperature sensor.
4-This analog value is applied to the analog to digital converter pin of the micro controller.
5-This analog value is converted to the digital value by the microcontroller using successive approximation method internally.
6-When the temperature is greater than the threshold value, microcontroller sends a command to the controller to switch the motor.
7-Thus fan starts rotating.


Component Description
LM35

The LM35 is an integrated circuit sensor that can be used to measure temperature. The output voltage of this sensor is proportional to the temperature in degree Centigrade. The output voltage of the LM35 will vary at a rate of 10mV per degree Celsius.

Usually, the range of the LM35 temperature sensor is from -55 deg C to +150 deg C. To measure this full range of temperatures i.e. from negative range to positive range, we need to connect an external resistor between the data pin and a negative supply of Vcc.

Any way, we are not going to consider the negative temperature range in this project. So, under normal operating conditions, we can measure the temperature in the range from +2 deg C to +150 deg C.

ADC

All the parameters of nature are of analog i.e. most of the data in the real world is characterised by analog signals. For instance, if the temperature of the room is measured.

The room temperature varies with time continuously. This measured signal, which continuously changes with time say from 1sec , 1.1sec , 1.2 sec and so on is called Analog signal.

In order to manipulate the real world data using a microprocessor or a microcontroller, we need to convert the analog signals to the digital signals, so that the processor or controller will be able to read, understand and manipulate the data.

Atmega8 has internal Analog to digital converter.

