<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>8-bit Processor Design – CSE 3203</title>
  <style>
    body {
      font-family: Arial, Helvetica, sans-serif;
      margin: 40px;
      line-height: 1.6;
      color: #222;
    }
    h1, h2, h3 {
      color: #003366;
    }
    h1 {
      border-bottom: 3px solid #003366;
      padding-bottom: 10px;
    }
    h2 {
      margin-top: 30px;
      border-bottom: 1px solid #ccc;
      padding-bottom: 5px;
    }
    ul {
      margin-left: 20px;
    }
    code {
      background: #f4f4f4;
      padding: 2px 6px;
      border-radius: 4px;
    }
    .note {
      background: #f9f9f9;
      border-left: 4px solid #003366;
      padding: 12px;
      margin: 20px 0;
    }
  </style>
</head>
<body>

<h1>8-bit Processor Design</h1>
<p><strong>Course:</strong> Computer Architecture and Organization (CSE 3203)</p>

<h2>Project Overview</h2>
<p>
This project presents the design and simulation of a simple <strong>8-bit processor</strong>
implemented using basic logic gates and atomic digital components. The processor was
designed according to the problem statement provided by the instructor and simulated
using <strong>Logisim</strong>.
</p>

<h2>Processor Architecture</h2>

<h3>CPU Word Size</h3>
<ul>
  <li>8-bit data path</li>
  <li>8-bit registers and buses</li>
</ul>

<h3>Arithmetic Logic Unit (ALU)</h3>
<p>
The ALU is designed using logic gates and supports the following operations:
</p>

<strong>Arithmetic Operations</strong>
<ul>
  <li>Addition</li>
  <li>Subtraction</li>
  <li>Multiplication</li>
  <li>Division</li>
</ul>

<strong>Logical Operations</strong>
<ul>
  <li>XOR</li>
  <li>NAND</li>
  <li>XNOR</li>
  <li>NOR</li>
</ul>

<p>
Both signed and unsigned integer operations are supported. No pre-built ALU components
were used in the design.
</p>

<h3>Instruction Set</h3>
<ul>
  <li>Total number of instructions: 8</li>
  <li>Supports one-address and two-address instruction formats</li>
  <li>Supports direct and indirect addressing modes</li>
  <li>No instruction performs two memory-to-memory operations</li>
</ul>

<h3>Control Unit</h3>
<p>
The control unit is implemented as a <strong>hardwired control unit</strong>. Control signals are
generated using combinational logic based on opcode and control sequencing signals.
</p>

<ul>
  <li>Implemented using AND, OR, NOT, and XOR gates</li>
  <li>Produces control signals for register transfer and ALU operations</li>
</ul>

<h3>Registers</h3>
<p>
The processor includes the following registers to support instruction execution:
</p>
<ul>
  <li>Program Counter (PC)</li>
  <li>Instruction Register (IR)</li>
  <li>Memory Address Register (MAR)</li>
  <li>Memory Buffer Register (MBR)</li>
  <li>Additional internal registers as required by the design</li>
</ul>

<h2>Memory Usage</h2>
<p>
The processor uses the built-in memory components available in Logisim. Custom cache
or main memory design is not included.
</p>

<h2>Simulation and Testing</h2>
<ul>
  <li>All components were simulated using Logisim</li>
  <li>ALU operations were verified using test inputs</li>
  <li>Instruction execution was observed through simulation</li>
</ul>

<h2>Project Structure</h2>
<pre>
8-bit-Processor/
│── ControlUnit.circ
│── ALU.circ
│── Adder.circ
│── Subtractor.circ
│── Processor.circ
│── README.html
</pre>

<h2>Conclusion</h2>
<p>
This project demonstrates the practical implementation of an 8-bit processor using
digital logic design principles. The design highlights the interaction between the
control unit, ALU, registers, and memory during instruction execution.
</p>

<p class="note">
<strong>Note:</strong> All components are designed using logic gates and basic digital elements,
and the processor was successfully simulated and demonstrated in Logisim.
</p>

<p>
<strong>Author:</strong> Samuel Terefe<br>
<strong>Department:</strong> Computer Science & Engineering
</p>

</body>
</html>
