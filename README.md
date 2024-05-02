# Measuring-PF-Energy-frequency-current-voltage-by-using-PZEM-004T-sensor
= Hardware Setup:
Connect the PZEM-004T module to the circuit you want to measure (usually in series with the load for current measurement and in parallel for voltage measurement).
Connect the I2C display (such as an OLED or LCD) to your microcontroller. Ensure it's properly wired and powered.
= Microcontroller Setup:
Initialize the I2C communication on your microcontroller.
Set up the PZEM-004T module for communication (if necessary, depending on the microcontroller and library you are using).
= Reading Electrical Parameters:
Read the current and voltage values from the PZEM-004T module using its communication protocol (usually serial communication like UART).
Read the frequency and power factor values if they are provided by the PZEM-004T module (some versions may not provide these directly).
= Displaying on I2C Display:
Convert the readings (current, voltage, frequency, power factor) into a format suitable for display (e.g., convert numerical values to strings).
Write the formatted values to the I2C display using the appropriate commands for your display module.
= Update Frequency:
Depending on your application requirements, decide how often you want to update the display with new readings. This could be continuously, at fixed intervals, or triggered by user input.
= Loop:
Continuously loop through steps 3 to 5 to update the display with the latest readingS.
