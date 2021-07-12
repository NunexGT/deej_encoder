# deej_encoder
Branch of the Deej Library by Omriharel but for use with encoders.

With this, you can now control your PC Sound, program by program, in a really practical way!

<img src="https://media.tenor.com/images/f4fc54c1cd7ead8a0891f584410b4c16/tenor.gif" width="350">
     
<h1>Links and references</h1>
SNR-Tech-Bytes Youtube Video: https://youtu.be/pkEw7x2GMIA

Original Deej work: https://github.com/omriharel/deej/blob/master/LICENSE

3D case made by SNR-Tech-Bytes: https://www.thingiverse.com/thing:4598978/

Arduino Program

<h1>Bill of Materials</h1>
Here´s what you need to buy for this project
<ul>
  <li>1 Arduino Nano or Uno (these are the recommended ones) 5V with ATmega 328</li>
  <li>(As much apps as you want to control, plus master) (5MAX) Rotary Encoders</li>
  <li>~30 Jumper cables (it´s better to have spare) Jumper Cables</li>
  <li>Welding Equipment (Machine and welds)</li>
 </ul>
<b>Optionals</b>
 <ul>
  <li>A BreadBoard (make sure that your breadboard has (+-) pins, if it doesn´t have is a PCB board, wich is useless in this case, unless to train welding)</li>
  <li>Led´s</li>
  <li>A case and/or material to make it</li>
 </ul>

<h1>Wiring Schematic</h1>

Rotary Encoders (NO VCC) with no BreadBoard (What I chose)
![](https://github.com/SuperX-dev/deej_encoder/blob/master/readme_resources/Wiring_Schematics/Rotary_Encoders_1_NoBreadBoard.jpg?raw=true)
Rotary Encoders (With VCC) with no BreadBoard
![](https://github.com/SuperX-dev/deej_encoder/blob/master/readme_resources/Wiring_Schematics/Rotary_Encoders_2_NoBreadBoard.jpg?raw=true)
*Note:<i>I can´t confirm if the vcc cconnected in this way will work properly because I used the first type of Rotary Encoders (Without VCC)</i>

Rotary Encoders (No VCC) with BreadBoard
![](https://github.com/SuperX-dev/deej_encoder/blob/master/readme_resources/Wiring_Schematics/Rotary_Encoders_1_BreadBoard.jpg?raw=true)
Rotary Encoders (With VCC) with BreadBoard
![](https://github.com/SuperX-dev/deej_encoder/blob/master/readme_resources/Wiring_Schematics/Rotary_Encoders_2_BreadBoard.jpg?raw=true)

<h4>Additional Notes</h4>
<ol>
  <li>The logic here is the same for the Arduino nano. The 5V pin can also be calles VCC or only "+". On arduino nano the digital ports (the ones on top in the Uno) have a D and then the number</li>
  <li>If you want more then 2 Encoders (which is very likely), continue the GND circuit (if not using BreadBoard) in the same way as these 2 are, just weld another cable to the  GND of the previous and continue</li>
</ol>

<h1>What to change in the .ino?</h1>
<ol>
  <li>First, change line 20-24. In the brackets, you´ll see some numbers in it, change according to the Digital Pin that you connected each Encoder. Don´t botter if the name of the apps you want to use don´t match with those. 
    <br>
    <i>Note:I can´t rember which one to put first and wich in second so the clockwise and anticlock wise positions are correct</i>
    <br>
    Example:
    <br>
    Code:
    <br>
    <img src="https://github.com/SuperX-dev/deej_encoder/blob/master/readme_resources/Wiring_Schematics/Code1.jpg?raw=true">
    <br>
    <img src="https://github.com/SuperX-dev/deej_encoder/blob/master/readme_resources/Wiring_Schematics/Code1schematics.jpg?raw=true"></li>
  <li>Between Lines 30-34. The same as the previous but for the Analog ones (change the number that comes after the A)</li>
  <li>Between lines 57-66. Lines that end with ".write(51)". This line means the the default volume of your computer when Deej is opened will be 51. Change that if you feel it´s too high (or too low who knows)</li>
  </ol>
  
  After that you can send the code to the arduino with the "<a href="https://www.microsoft.com/pt-pt/p/arduino-ide/9nblggh4rsd8?ocid=badge&rtc=1&activetab=pivot:overviewtab"> Arduino IDE</a>" 
  
  <h1>Case Assemblage Suggestions</h1>
Now, the case really depends on your taste and what you want to do. You allways have the option to 3D print it, there are lot´s of Deej project files ready to print. But not everyone has access to a 3D printer and using a Shoe boc in your setup, is just not great.
  So if you don´t have a case laying around or something like that, my friends gave me the advice to buy Acrylic, cut it and the with all the faces cutted glue them together with the help of some screws to support it. Make some holes for the Encodes and you should be done. There are also colored Acrylic so this is a good solution.
  And of course, there are also other ways of doing it.
  
  </h1>
  
<h1>Thank You</h1>
This is all, thank you for reading this. Don´t forget to check out the <a href="https://github.com/omriharel/deej">Deej Original Repo</a>
<br>
Also, don´t forget to check out how to install and configure Deej: https://github.com/omriharel/deej#how-to-run


