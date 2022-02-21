# M2-EmbSys
Embedded System
Based on IOT Module And it depends on three parts -

1) Automation of BP monitoring Device.
 2) Fetching the data from the BP machine.
 3) Uploading the data to Things Board.

1) Automation of BP monitoring Device -
Automation of BP monitoring Device is completely achieved by 2N222 NPN Transistor, D1 mini, Blynk application.
2N222 is a Bipolar junction transistor and it is generally used of switching or amplification purpose [10].
This NPN transistor is Generally low power, low to medium current, medium voltage, and this transistor works very well at high speeds [11].  NPN Transistor has three terminals Base, emitter and collector and it offers current like 800mA, so that it is necessary to use where low to medium current is necessary.[10][11].
D1 Mini is a Wi-Fi enable microcontroller. Internet of things has ability to sense devices and collect the data from surrounding.[3]. Main functionality of d1 mini is methods like home automation can be controlled by d1 mini from remote location.[12]
The microcontroller will act as a main processing unit such as giving a command to the BP machine to turn ON and OFF, retrieving the data from electronically erasable programmable read-only memory (EEPROM) of the BP monitoring machine and feeding the data to the Things Board which is a cloud platform.
Blynk app allows you to build interfaces for controlling projects from android and iOS devices.[13]
 In this process, the traditional push switch is replaced by 2N2222 NPN transistor. It will emulate the switching process. The base pin of the transistor is connected to the digital pin “D4” of the D1 Mini, the transistor will be triggered by a microcontroller in a certain interval of time like, e.g., 5 minutes, 10 minutes, 20 minutes, 30 minutes, 60 minutes, 120 minutes and so on, this interval can be set with the help of Blynk Application. If the medical practitioner suggests taking the blood pressure in every 60 min throughout the day, this interval is set with the help of Blynk Application then the transistor will get triggered every 60 min in order to turn ON the BP monitoring device. Figure shows the circuit diagram of the proposed BP monitoring device.
2) Fetching the data from the BP machine -
After the measurement is done the is stored into EEPROM of the device. EEPROM Stands for electrically erasable programmable read – only memory [13]. EEPROM allows user to erase and reprogram data in an application.[13][14].
In next generation health care system, the data is fetched by the microcontroller via. I2C protocol. This circuit diagram shows the transistor which emulates the switching process by replacing the push switch of the device. Transistor is triggered periodically in a certain set interval of time. After the measurement is done, the data is retrieved from EEPROM the BP machine using I2C protocol where Serial clock line (SCL) pin of EEPROM is connected to pin D1 and Serial data line (SDA) is connected to pin D2 of the microcontroller. Buzzer is connected to the D3 pin, beeps indicating measurement is done. Figure depicts the data fetching from the proposed BP monitoring device.

3) Uploading the data to the Things Board -

Iot provides various platforms for data collection, processing, visualization management [8]. Things board is a one of the most famous open-source cloud platforms which provides data collection and processing [8].
Things board allows defining rules, that can be applied to incoming messages and plugins [8].
The visualization functionality provided by iot via things board convert data into knowledge which is critical in fast decision making [3]. Things is use to monitor and collect data from iot device [9]. things board has dashboard to provide number of options to virtualize data in the form of line, chart [9]. The visualization functionality provided by iot via things board convert data into knowledge which is critical in fast decision making [3].
•	FUTURE SCOPE
1.	 In the Covid19 pandemic, a particular challenge is the ongoing flow of patients, a significant proportion of which must be transferred to the intensive care unit (ICU) due to mechanical ventilation system failure. Early detection of  patients who may need to be transferred to the ICU is an important step in the management of COVID 19 patients. To solve this problem, we are using the EWS system for early detection of COVID 19 patients who need to be admitted to the ICU.
2.	In the future, this ML-based EWS system can be deployed in all hospitals to improve the detection of patients at risk of  unplanned ICU transfers. This will prevent events that lead to  high  mortality. You may also be able to reduce costs by shortening your stay in the ICU  and reducing treatment. 
3.	This type of system can  be used by patients with disabilities and in places where transportation is not readily available. If  such a system is present in these dangerous locations, they can get  early warnings that give them a little more time to take precautions so that patients can get  medical assistance in time.
