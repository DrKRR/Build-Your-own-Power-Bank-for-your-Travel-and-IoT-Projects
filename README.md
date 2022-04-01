# Build-Your-own-Power-Bank-for-your-Travel-and-IoT-Projects
This Project explains how to build a cost-effective power bank for mobile phones during travel and for powering up the IoT Projects as **DIY** (Do It Yourself).
</br>
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/160660232-8ecccfd3-02de-4168-b503-be08534eb20c.png"
" width = "250" height = "150"></p>  
On highways, there is every likelyhood that mobile towers are built in such a way that continuous signals are available for the mobile data and hence battery will last for more time. But during normal road and train journies, our travel passes through ups, downs, curvatures and amidst big hills. During these times, no mobile signals will be available or the signals will be very feeble. Thus, we travel constantly in and out of a tower’s range and into the next one . The device (mobile or any electronic device that uses data) ping each tower when entering and leaving it’s range. Signal searching becomes more aggressive when signals from other cell towers (not registered with the SIM card inside the mobile) are within the range of the mobile. The radio inside the device (transmitter and receiver section on the mobile), uses more power during such signal fluctuations to maintain the network level, that results in more power usage which leads to battery drain. Worst case being, the mobile switches off before reaching the destination point. Carrying a power bank(s) in such scenarios will avoid frustration, especially, when there are limited charging points. </br>
<br /> 
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/160793549-6b27235e-b573-4e41-8f45-3ac26a8a0dd7.png"
" width = "250" height = "150"></p> 

Readymade power banks are available on the market. But, they are not only costly but also the troubleshooting is a difficult task. In the light of this fact, I present DIY power bank which is cost-effective and also easy to replace when there is a problem with the battery or
charging electronics. It works well during travel and also can be used for testing embedded and IoT projects.
## MATERIALS AND METHOD ##
Power bank mainly consists of three parts:
* Lithium-ion or Lithium-polymer battery
* Battery charging electronic circuit
* Case to hold both the above
### BATTERY ###
In this explanation I concentrate on Lithium-ion batteries, due to its popularity. In fact, the Nobel Prize in *Chemistry* for the year 2019 is being shared by three scientists for their invention: *"Development of Lithium-ion Batteries"*
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/160837059-ee821707-7dd2-401d-8243-1fef6037b8f7.png"
" width = "350" height = "150"></p>  
  
Certain advantages of Li-ion batteries include:
* lighter and more compact compared Lead-acid batteries still found in cars
* rechargeable, unlike disposable zinc and alkaline batteries used in medical-electronic devices and toys
* unlike Nickel-Cadmium rechargeable batteries that contains toxic Cd, Li-ion batteries doesn't contain toxic metal
* Li-ion battery doesn't have "memory effect", which is prevalant in Ni-Cd cells
* Li-ion cells are availble in portable sizes and shapes: cylindrical and rectangular 
  
Following are the images of Li-ion batteries used in power banks, laptops, mobile phones etc.
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/160846408-ff763e45-f66e-43a1-a5cc-887449535927.png"
" width = "370" height = "150"></p> 

In the above, Li-ion batteries shown in (a) and (b) are used in mobile phones, tablets while that are used in power banks and laptops is shown in (c).
Li-ion batteries used in power banks and laptop's power supplies, and general power supplies are numbered as 18650 with 3.7V and current ratings is shown below:
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/160850211-4b6df1cf-ea8a-4e64-829f-da6e08621219.png"
" width = "300" height = "175"></p> 

The cross-sectional views of both type of batteries are shown below. Working of the battery is out of the scope this presentation.
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/160853692-91fc5f2e-a168-4bb7-9b11-0efbe46d79d6.png"
" width = "400" height = "200"></p> 

### ELECTRONIC CHARGING CIRCUIT ###

Charging a LI-ion 18650 battery can be accomplished by different methods. Due to the developments in VLSI technology, many charging circuits are coming in the form of ICs. These ICs in conjunction with PCB mountable miniature L,C,R components will be used as battery chargers. Certain popular charger ICs are:
* HT4928S
* SW2808S
* 134N3P
* MC34063A
* TP4056
* HX3589
* ST6845

The Hotchip HT4928S and SW2808S are very popular among these chips. Further, these ICs are widely used in power bank circuits.
The HT4928S is a highly integrated mobile power supply management system (MPSMS). It has a built-in charge management module, LED(s) indicator module, and a boost discharge management module. It is available in 8-pin SOP package. This chip is described as: 
*"5V-Step-Up-Power-Module-Lithium-Battery-Charging-Protection-Board-Boost-Converter-LED-Display-USB"*.
The inernal architecture and the pin configuration of HT4928S are shown below: 
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/161175007-c8852b07-84f9-42e3-9e33-542a06ee673d.png"
" width = "450" height = "250"></p> 
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/161177608-eda7f1a1-fc60-4d17-85a6-d181bbba34e5.png"
" width = "450" height = "250"></p>

The circuit diagram and the end product wherein the SW2808S and supporting components soldered in the form of PCB are shown below:
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/161178284-155f1767-2805-4d73-b057-f5c7d2d09cbd.png"
" width = "800" height = "450"></p> 
  
Now, it is time to understand assembling of the individual components. In the above figure I have shown the assembled PCB that goes in to the design of power bank. The assembly consisting of the aluminium casing, battery holder is shown in the following figure. 
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/161191220-87cd2f68-90ac-44c4-86fb-bb032b5ca5d5.png"
" width = "450" height = "350"></p> 

A plate is soldered to the PCB that acts as positive terminal, and one end of a long wire is soldered to the negative terminal of the PCB and the other end of the wire is wound in a spiral shape that fits in to the plastic battery holder. The spacing between the positive plate and spiral end is such, the 18650 battery just fits exactly as shown in the figure below. The approximate size of the battery is 6.5cm. in length and 1.7cm. in diameter. Power bank constructed in such a way gives an output of 5V at 1A.
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/161208796-8a57a0ae-d422-4e6d-b468-fd16db803243.png"
" width = "500" height = "350"></p> 
  
The power bank shown above can be charged with mobile chargers with micro USB2.0B termination. I used Motorola and Redmi mobile chargers (shown below) to successfully charge the power banks. Check your charger specifications before use. Use only elegible chargers to charge your power bank, otherwise it may lead to explosion of battery/catching up fire/spoiling of the charger circuit/charger itself.
<p align = "center"><img src="https://user-images.githubusercontent.com/93868543/161237509-d551398f-d58d-4888-8ca1-ad7fa3a66f67.png"
" width = "450" height = "350"></p>
Such Li-ion batteries with high charge density and long life are used in Tesla cars. The following video (YouTube) shows the working of Li-ion battery and its use in Tesla cars.

<p align = "center"> [(https://www.youtube.com/watch?v=VxMM4g2Sk8U)] <p/> 

### DISCLAIMER ###
Before you work with this project in any way, please make sure you understand what you are doing. Electronic circuits and batteries
can be harmful and dangerous when not used with proper care and administration. 

Trying to duplicate or use this project in any way you agree that you are using it at your own risk and no body can be held responsible or accountable for any damage or harm that might be caused due to your use of this project

" USE THE PROJECT AT YOUR OWN RISK "
