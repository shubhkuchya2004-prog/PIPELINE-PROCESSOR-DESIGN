# PIPELINE-PROCESSOR-DESIGN

*COMPANY* : CODTECH IT SOLUTIONS

*NAME* : SHUBH KUCHYA

*INTERN ID* : CT04DR1218

*DOMAIN* : VLSI

*DURATION* : 4 WEEKS

*MENTOR* : NEELA SANTOSH

The task involves designing and simulating a 4-stage pipelined processor capable of executing basic arithmetic and memory-access instructions. The processor follows a simplified RISC architecture and supports the following operations:

ADD – register-to-register addition

SUB – register-to-register subtraction

LOAD – memory load using base register + immediate addressing

The processor datapath is divided into four pipeline stages:

Instruction Fetch (IF) – Retrieves the instruction from program memory.

Instruction Decode (ID) – Decodes the instruction, identifies opcode, reads register operands, and sign-extends immediate values.

Execute (EX) – Performs ALU operations for ADD and SUB or computes the effective address for LOAD.

Write Back (WB) – Writes the ALU or memory result back into the destination register.

Intermediate values are passed between stages using pipeline registers (IF/ID, ID/EX, EX/WB), enabling multiple instructions to be processed simultaneously. As a result, once the pipeline is filled, one instruction completes during every clock cycle, improving performance compared to a non-pipelined processor.

A Verilog testbench was developed to simulate the processor’s behavior and display the internal values of each pipeline stage during execution. The simulation verifies correct instruction flow through all stages, proper ALU computations, and accurate data loading from memory. Observing the stage-by-stage transitions in the simulation confirms that the pipelined processor operates functionally and that overlapping execution of instructions is achieved.
