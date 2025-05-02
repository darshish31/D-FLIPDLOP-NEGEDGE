# D-FLIPDLOP-NEGEDGE

**AIM:**

To implement  D flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**D Flip-Flop**

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

**Procedure**

Create the D flip-flop module in Verilog with inputs D, clk and outputs Q, Qbar.

Define behavior using always @(posedge clk) to assign Q = D and Qbar = ~D.

Write a testbench to apply different D values with clock transitions.

Simulate and monitor output changes (Q, Qbar) on each clock edge.

Verify outputs against the D flip-flop truth table to confirm correct functionality.

**PROGRAM**

![program](https://github.com/user-attachments/assets/9c777589-e90b-4bf1-ad2c-8aae8bafe4f8)

**RTL LOGIC FOR FLIPFLOPS**

![simulation](https://github.com/user-attachments/assets/33f3098c-cfe2-401b-b96f-d217008e9047)

**TIMING DIGRAMS FOR FLIP FLOPS**

![waveform](https://github.com/user-attachments/assets/94e7e421-6e16-4e70-a57b-69278e72e80f)

**RESULTS**

The D flip-flop was successfully implemented and validated in Verilog, with outputs accurately reflecting its functional truth table.
