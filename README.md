# mips-lab-2--mips-5-stage-pipeline-simulator-solved
**TO GET THIS SOLUTION VISIT:** [MIPS Lab 2- MIPS 5 Stage Pipeline Simulator Solved](https://www.ankitcodinghub.com/product/mips-lab-2-mips-5-stage-pipeline-simulator-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91278&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;MIPS Lab 2- MIPS 5 Stage Pipeline Simulator Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Lab 2: MIPS 5 Stage Pipeline Simulato

Upload your code to BrightSpace as a zip folder named: &lt;netID_student1&gt;_&lt;netID_student2&gt; where &lt;netID_student1/2&gt; are each student’s netID.

In this Lab assignment, you will implement a cycle-accurate simulator for a 5-stage pipelined MIPS processor in C++. The simulator supports a subset of the MIPS instruction set and should model the execution of each instruction cycle by cycle.

The MIPS program is provided to the simulator as a text file “imem.txt” file that is used to initialize the Instruction Memory. Each line of the file corresponds to a Byte stored in the Instruction Memory in binary format, with the first line at address 0, the next line at address 1 and so on. Four contiguous lines correspond to a whole instruction. Note that the words stored in memory are in “Big-Endian” format, meaning that the most significant byte is stored first.

The Data Memory is initialized using the “dmem.txt” file. The format of the stored words is the same as the Instruction Memory. As with the instruction memory, the data memory addresses also begin at 0 and increment by one in each line.

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
The instructions to be supported and their encodings are shown in Table 1. Note that all instructions, except for “halt”, exist in the MIPS ISA. The MIPS Green Sheet defines the semantics of each instruction.

For the purposes of this lab only, we will assume that the beq (branch-if-qual) instruction operates like a bne (branch-if-not-equal) instruction. In other words, in your implementations you will assume that the beq jumps to the branch address if 𝑅[𝑟𝑠] ≠ 𝑅[𝑟𝑡] and jumps to PC+4 otherwise, i.e., if 𝑅[𝑟𝑠] = 𝑅[𝑟𝑡].

(Note that a real beq instruction would operate in the opposite fashion, that is, it will jump to the branch address if 𝑅[𝑟𝑠] = 𝑅[𝑟𝑡] and to PC+4 otherwise. The reason we had to make this modification for this lab is because to implement loops we actually need the bne instruction.)

</div>
</div>
<div class="layoutArea">
<div class="column">
Instruction

Addu Subu Lw Sw Beq Halt

</div>
<div class="column">
Format

R-type R-type I-Type I-type I-type Custom

</div>
<div class="column">
OpCode (hex)

00 00 23 2B 04 FF

</div>
<div class="column">
Function code (hex)

21 23 – – – –

</div>
</div>
<div class="layoutArea">
<div class="column">
Pipeline Structure

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Your MIPS pipeline has the following 5 stages:

<ol>
<li>Fetch (IF): fetches an instruction from instruction memory. Updates PC.</li>
<li>Decode (ID/RF): reads from the register RF and generates control signals required in
subsequent stages. In addition, branches are resolved in this stage by checking for the

branch condition and computing the effective address.
</li>
<li>Execute (EX): performs an ALU operation.</li>
<li>Memory (MEM): loads or stores a 32-bit word from data memory.</li>
<li>Writeback (WB): writes back data to the RF.</li>
</ol>
Your simulator can make use of the same RF, IMEM and DMEM classes that you used for Lab0. Complete implementations of these classes are provided for you in the skeleton code.

Note that we have not defined an ALU class since, for this lab, the ALU is simple and only needs to perform adds and subtracts.

Each pipeline stages takes inputs from flip-flops. The input flip-flops for each pipeline stage are described in the tables below.

</div>
</div>
<div class="layoutArea">
<div class="column">
IF Stage Input Flip-Flops

Flip-Flop Name Bit-width

PC 32 nop 1

IF/ID Stage Flip-Flops

Flip-Flop Name Bit-width

Instr 32 nop 1

</div>
<div class="column">
Functionality

Current value of PC

If set, IF stage performs a nop

Functionality

32b instruction read from Imem If set, ID stage performs a nop

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
ID/EXE Stage Flip-Flops

Flip-Flop Name Bit-width

</div>
<div class="column">
Functionality

</div>
</div>
<div class="layoutArea">
<div class="column">
Read_data1, Read_data2

</div>
<div class="column">
32 32b data values read from RF

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Rs, Rt

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Addresses of source registers rs, rt. Note these are defined for both R-type and I-type instrucions

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Wrt_reg_addr

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Address of the instruction’s destination register. Don’t care is the instruction doesn’t update RF

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
Alu_op 1 Is_I_type 1 Wrt_enable 1 Rd_mem, Wr_mem 1 Nop 1

</div>
<div class="column">
Set for addu, lw, sw; unset for subu

Set if the instruction is I-type

Set if instruction updates RF

Rd_mem set for lw and wrt_mem set for sw instructions. If set, EXE stage performs a nop

</div>
</div>
<div class="layoutArea">
<div class="column">
EXE/MEM Stage Flip-Flops

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
Flip-Flop Name Bit-width

</div>
<div class="column">
Functionality

32b ALU result, don’t care for beq

</div>
</div>
<div class="layoutArea">
<div class="column">
ALU_result

</div>
<div class="column">
32

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Store_data

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
32

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
32b value to be stored in DMEM for sw instruction. Don’t care otherwise

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Rs, Rt

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Addresses of source registers rs, rt. Note that these are defined for both R-type and I- type instructions.

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Wrt_reg_addr

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Address of the instruction’s destination register. Don’t care if the instruction doesn’t update the RF.

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
Wrt_enable 1 Rd_mem, Wr_mem 1 Nop 1

WB Stage Input Flip-Flops

Flip-Flop Name Bit-width

</div>
<div class="column">
Set if instruction updates RF

Rd_mem set for lw and wrt_mem set for sw instructions. If set, EXE stage performs a nop

Functionality

32b value to be written vack to RF. Don’t care for sw and beq.

Set if instruction updates RF

If set, EXE stage performs a nop

</div>
</div>
<div class="layoutArea">
<div class="column">
Wrt_data

</div>
<div class="column">
32

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Rs, Rt

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Addresses of source registers rs, rt. Note that these are defined for both R-type and I- type instructions.

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Wrt_reg_addr

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Address of the instruction’s destination register. Don’t care if the instruction doesn’t update the RF.

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
Wrt_enable 1 Nop 1

Dealing with Hazards

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
Your processor must deal with two types of hazards.

<ol>
<li>RAW Hazards: RAW hazards are dealt with using either only forwarding (if possible) or, if not, using stalling + forwarding. You must follow the mechanisms described in Lecture to deal RAW hazards.</li>
<li>Control Flow Hazards: You will assume that branch conditions are resolved in the ID/RF</li>
</ol>
stage of the pipeline. Your processor deals with beq instructions as follows:

<ol>
<li>a) &nbsp;Branches are always assumed to be NOT TAKEN. That is, when a beq is fetched in the IF stage, the PC is speculatively updated as PC+4.</li>
<li>b) &nbsp;Branch conditions are resolved in the ID/RF stage.

To make your life easier, will ensure that every beq instruction has no RAW dependency with its previous two instructions. In other words, you do NOT have to deal with RAW hazards for branches!</li>
<li>c) &nbsp;Two operations are performed in the ID/RF stage: (i) Read_data1 and Read_data2 are compared to determine the branch outcome; (ii) the effective branch address is computed.</li>
<li>d) &nbsp;If the branch is NOT TAKEN, execution proceeds normally. However, if the branch is TAKEN, the speculatively fetched instruction from PC+4 is quashed in its ID/RF stage using the nop bit and the next instruction is fetched from the effective branch address. Execution now proceeds normally.</li>
</ol>
The nop bit

The nop bit for any stage indicates whether it is performing a valid operation in the current clock cycle. The nop bit for the IF stage is initialized to 0 and for all other stages is initialized to 1. (This is because in the first clock cycle, only the IF stage performs a valid operation.)

In the absence of hazards, the value of the nop bit for a stage in the current clock cycle is equal to the nop bit of the prior stage in the previous clock cycle.

However, the nop bit is also used to implement stall that result from a RAW hazard or to quash speculatively fetched instructions if the branch condition evaluates to TAKEN. See Lecture 6 slides for more details on implementing stalls and quashing instructions.

The HALT Instruction

The halt instruction is a “custom” instruction we introduced so you know when to stop the simulation. When a HALT instruction is fetched in IF stage at cycle N, the nop bit of the IF stage in the next clock cycle (cycle N+1) is set to 1 and subsequently stays at 1. The nop bit of the ID/RF stage is set to 1 in cycle N+1 and subsequently stays at 1. The nop bit of the EX stage is set to 1 in cycle N+2 and subsequently stays at 1. The nop bit of the MEM stage is set to 1 in cycle N+3 and subsequently stays at 1. The nop bit of the WB stage is set to 1 in cycle N+4 and subsequently stays at 1.

At the end of each clock cycle the simulator checks to see if the nop bit of each stage is 1. If so, the simulation halts. Note that this logic is already implemented in the skeleton code provided to you.

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
What to Output

Your simulator will output the values of all flip-flops at the end of each clock cycle. Further, when the simulation terminates, the simulator also outputs the state of the RF and Dmem. The skeleton code already prints out everything that your simulator needs to output. Do not modify this code.

&nbsp;

</div>
</div>
</div>
