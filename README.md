Download Link: https://assignmentchef.com/product/solved-cs223-laboratory-assignment-1-digital-circuits-logic-to-gates
<br>
<h1>Preliminary Work (30 pts)</h1>

(You should do this part before coming to lab).

Physical gates are built out of transistors, and require physical signals that use correct voltage levels for inputs and produce physical signals with correct voltage levels for outputs. To work correctly, the transistor circuits that comprise a gate must have connections to a voltage supply and to ground. For example, in the case of 74-series logic circuits used in this lab, the supply voltage (Vcc) must be 5 volts. In these integrated circuit packages, several gates are contained. Search Google specifying that gate number and its function (e.g. “7486 XOR gate”) for pin connection diagrams, such as the pin diagram shown in Figure 1. You must have the pin diagrams for each gate you want to use, in order to do the following tasks. You can find pinout of rest of 74-series gates here: <a href="http://www.qsl.net/on7pc/datasheet/ttl7400/7400family.pdf">http://www.qsl.net/on7pc/datasheet/ttl7400/7400family.pdf</a><a href="http://www.qsl.net/on7pc/datasheet/ttl7400/7400family.pdf">.</a> Other gates you need today are: 7408 quad 2-input AND gate, 7432 quad 2-input OR gate, and 7404 six INVERTER.

<h2>Figure 1: 7486 Quad 2-input XOR gates</h2>




First, read the document posted in Moodle: “Circuit Schematic versus Logic Diagram”. Then, using the logic diagram of Half Adder in Figure 2, draw a <em><u>circuit schematic</u></em> of the digital circuit you will build. This should include <strong>pin numbers</strong> marked on the inputs and outputs of all the gates, <strong>part numbers </strong>(IC’s code) of the IC package marked on each gate, plus <strong>power and ground connections</strong> marked on the side of the drawing. After that, draw the <em><u>circuit schematics</u></em> for Half Subtractor shown in Figure 3 and Lab Calculator given in Figure 4. <u>Upload your schematics to Moodle as a</u> <u>pdf file before your lab session starts</u>. Late submissions won’t be accepted. You are advised to draw using tools like draw.io, but you are allowed to draw by hand and then scan/take a photo, as long as it is readable.

Figure 2: Half Adder

<h2>Figure 3: Half Subtractor</h2>







<table width="548">

 <tbody>

  <tr>

   <td width="113"><strong>Control Input C </strong></td>

   <td width="83"><strong>Function </strong></td>

   <td width="117"><strong>Function </strong></td>

   <td width="110"><strong>Output Y </strong></td>

   <td width="125"><strong>Output Z </strong></td>

  </tr>

  <tr>

   <td width="113">0</td>

   <td width="83">A + B</td>

   <td width="117">Half Adder</td>

   <td width="110">Sum (S)</td>

   <td width="125">Carry Out (Co)</td>

  </tr>

  <tr>

   <td width="113">1</td>

   <td width="83">A – B</td>

   <td width="117">Half Subtractor</td>

   <td width="110">Difference (D)</td>

   <td width="125">Borrow out (Bo)</td>

  </tr>

 </tbody>

</table>







<strong>Figure 4: Lab Calculator </strong>

<h1>Recommendations</h1>

In CS223 labs, you build circuits by ICs and later by FPGA. It is better to obey some simple rules to avoid damaging electronic parts or confusing yourself with debugging your circuit.

<ul>

 <li>Avoid touching IC or FPGA pins directly by your hand. Static electricity of your body can damage them permanently.</li>

 <li>The white board which you setup your circuit on it, is called “breadboard”. Search in internet and find out how its pins are connected internally.</li>

 <li>Postpone connecting power pins (Vcc and ground) to last step. Check circuit connections and if everything seems ok then connect power pins.</li>

 <li>For easier debugging of circuits, always follow a wire color convention. For example, always use black or white wire for ground and red wire for Vcc.</li>

 <li>If LED’s light is weak, or if the IC’s package is very hot (you can touch plastic part) you have a problem in the power pin connections (short circuit, connecting Vcc wire to ground pin, etc).</li>

</ul>




<h1>Part 1: Building Half Adder &amp; Subtractor (40 pts)<sub>  </sub></h1>

<ul>

 <li>Ask the TA or Tutor to come and check your schematics. <em>Do not proceed to the next step until </em>you have verified that your circuit schematics are correct, and the TA or Tutor has approved them.</li>

 <li>Using your circuit schematics for half adder and half subtractor, build the circuits step-by-step, following the Digital Circuit Suggestions document given in Moodle and recommendations above. Connect the inputs to switches on the logic board. Connect the outputs of your logic circuits to LEDs on the logic board. Don’t forget to connect VCC power and GND ground to the VCC and GND pins of IC packages.</li>

 <li>Make a test probe by connecting another LED on the logic board to one end of a long wire, whose other end will be used to touch circuit points and “see” the logic values. A full voltage level ~5 V will cause the LED to shine brightly; a 0 V level will not light up the LED. A low light output from the LED means that the voltage being sensed is in between logic 0 and logic 1, meaning something is WRONG with your circuit.</li>

 <li>Now draw the truth tables for the 2-input 2-output logic circuits that you have made and fill in the left-hand (input) side in standard binary counting order. For each row, apply the input combinations by adjusting the switches, and measure the output. Use this information to complete the truth table, filling in the right-hand (output) side.</li>

 <li>Compare your measured truth tables that you obtained from the circuits, with the ones given below. If there are no discrepancies, then it means that your logic circuits have worked as predicted. Ask the TA or Tutor to come and verify this. When the TA or Tutor has checked your circuits, you are done with this part.</li>

</ul>

<strong>                                             </strong><strong> </strong>

<strong>   Figure 5: Truth table of a half adder                            Figure 6: Truth table of a half subtractor </strong>

<h1>Part 2: Building Lab Calculator (30 pts)</h1>

<ul>

 <li>Ask the TA or Tutor to come and check your schematic for the lab calculator. <em>Do not proceed to the next step until </em>you have verified that your circuit schematic is correct, and the TA or Tutor has approved it.</li>

 <li>Using your circuit schematic, build the circuit following the Digital Circuit Suggestions given in Moodle. Connect the inputs to switches on the logic board. Connect the outputs of your logic circuit to LEDs on the logic board. Don’t forget to connect VCC power and GND ground to the VCC and GND pins of IC packages.</li>

 <li>As you did in Part 1, test and verify that your built circuit is working correctly as a calculator that produces the outputs of a half adder or half subtractor depending on the value of C input. Compare your measured truth table with the one given below. If there are no discrepancies, then it means that your logic circuit is working correctly, ask the TA or Tutor to come and verify this. When the TA or Tutor has checked your circuit, you are done with this part.</li>

</ul>

<table width="189">

 <tbody>

  <tr>

   <td width="52"><strong>C </strong></td>

   <td width="38"><strong>A </strong></td>

   <td width="23"><strong>B </strong></td>

   <td width="53"><strong>Y </strong></td>

   <td width="23"><strong>Z </strong></td>

  </tr>

  <tr>

   <td width="52">0</td>

   <td width="38">0</td>

   <td width="23">0</td>

   <td width="53">0</td>

   <td width="23">0</td>

  </tr>

  <tr>

   <td width="52">0</td>

   <td width="38">0</td>

   <td width="23">1</td>

   <td width="53">1</td>

   <td width="23">0</td>

  </tr>

  <tr>

   <td width="52">0</td>

   <td width="38">1</td>

   <td width="23">0</td>

   <td width="53">1</td>

   <td width="23">0</td>

  </tr>

  <tr>

   <td width="52">0</td>

   <td width="38">1</td>

   <td width="23">1</td>

   <td width="53">0</td>

   <td width="23">1</td>

  </tr>

  <tr>

   <td width="52">1</td>

   <td width="38">0</td>

   <td width="23">0</td>

   <td width="53">0</td>

   <td width="23">0</td>

  </tr>

  <tr>

   <td width="52">1</td>

   <td width="38">0</td>

   <td width="23">1</td>

   <td width="53">1</td>

   <td width="23">1</td>

  </tr>

  <tr>

   <td width="52">1</td>

   <td width="38">1</td>

   <td width="23">0</td>

   <td width="53">1</td>

   <td width="23">0</td>

  </tr>

  <tr>

   <td width="52">1</td>

   <td width="38">1</td>

   <td width="23">1</td>

   <td width="53">0</td>

   <td width="23">0</td>

  </tr>

 </tbody>

</table>

<strong>Figure 7: Truth table of the Lab Calculator </strong>




<ol>

 <li></li>

</ol>