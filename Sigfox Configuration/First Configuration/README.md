# Sigfox

The first step to be able to use the Sigfox services, you must have the necessary hardware like the ones shown on the official website: https://partners.sigfox.com/products/device

In this project, we are using a Pycom FiPy Board, which in addition to the services of LoRa, LTE Cat-M1 / NB-IoT, Wifi, Etc... has embeded the Sigfox connectivity, in addition to a free subscription for two years to their platform.

# Before starting

The first fundamental step to use the Sigfox technology, is to check that they have coverage in your area, because if they do not have it, it does not make sense to follow this tutorial.

https://www.sigfox.com/en/coverage

If there is coverage in your area, then the next step will be to review your coverage area code, which will have to be placed later in your code to be able to send packages.

https://radiocrafts.com/kb/what-is-a-sigfox-zone/

# How to configure my device?

Each of the different models of boards that use this technology have different ways to register the component and activate the Sigfox service, but in general they have some points in common.

1.- Perform the firmware update of the device to the latest version.

1.1- In the specific case of the Pycom board, it is necessary to update it through the page Pybytes and also use the software to update it. 

1.11- WebPage:  https://pybytes.pycom.io/

1.12- Firmware: https://docs.pycom.io/chapter/gettingstarted/installation/firmwaretool.html


2.- Obtain the Device ID and PAC number from your board.

2.1- For the Pycom board this is easily obtained after doing a software update.

2.11-Automatically the program indicates both numbers for the LoRa and Sigfox registration (in case you want to save it for another project).


3.- Make the registration of your hardware on the official Sigfox website.

3.1- The registration on the page is very simple, it is also good practice to give some information of your project in the registry to support the company, and help them to improve their services.

3.11- WebPage: https://buy.sigfox.com/ 

3.111- Clic in the button "Activate my DevKit"
<img src="https://image.ibb.co/kT5DpT/68747470733a2f2f707265766965772e6962622e636f2f6275437774642f436170747572615f64655f70616e74616c6c615f64655f323031385f30375f32315f30325f30375f31342e706e67.png" width="800">

3.112- Complete the registration.


4.- Enter the backend page of the sigfox platform to be able to upload your first value to the system. (If you do not send your first value to the platform before 4 months, the system deactivates your free account). WebPage:https://backend.sigfox.com/device/list

4.1.- To be able to visualize your first value on the page you have to go to the following path:
Device - [ID] - Messages

(On this page you will see the values that you send.)

Reference Images:

<img src="https://image.ibb.co/go0eUT/68747470733a2f2f707265766965772e6962622e636f2f6e68365a654a2f436170747572615f64655f70616e74616c6c615f64655f323031385f30375f32315f30325f33395f32342e706e67.png" width="800">
<img src="https://image.ibb.co/ijVPw8/68747470733a2f2f707265766965772e6962622e636f2f666e625436792f436170747572615f64655f70616e74616c6c615f64655f323031385f30375f32315f30325f34315f33312e706e67.png" width="800">

5.- Make the corresponding code for the board you are using to make the first data upload to the platform. (In this folder we provide the codes to send the first data from Pycom).

Link: https://github.com/EddOliver/AggroFox/tree/master/Sigfox%20Configuration/First%20Configuration/Pycom%20Test%20Code

# Next Step

After having made the first configuration and tested the Sigfox module (in this case the Pycom), follow the steps in the following link:

Link: https://github.com/EddOliver/AggroFox/tree/master/Sigfox%20Configuration/Aggrofox%20Conf

Official Pycom WebPage Documents: https://docs.pycom.io/chapter/firmwareapi/pycom/network/sigfox.html
