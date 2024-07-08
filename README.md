# Tiny CPU Architecture

Introduction : Central processing unit (CPU) Architecture is the electronic circuitry within a computer that carries out the instructions of a computer program by performing the basic arithmetic, logical, control and input/output (I/O) operations specified by the instructions.

Objective : Make a project on RTL Design Synthesis of a basic CPU Architecture which includes a CPU and Memory.

Methodology : The design is based on the concept of finite state machines. The system works via synchronous read-write cycles. Pipeline helps to send next address of instruction to memory while processing current instructions. The RTL code is also verified via testbench and timing diagrams.
  
Technical Aspects : The CPU structure consists of PC(Program Counter), 2 Registers A(acting as accumulator) & B, and various Opcodes. The opcodes used are NOP, MOVA, MOVB, MOVAM, MOVBM, MOVM, ADD, SUB, MULT, DIV and HALT. The Memory works via synchronous read-write cycles. The fast pipeline involves states like initialization, fetch-decode, data transfer. Fetch and Decode makes PC increment and drives ADDR to memory to fetch next instruction while also reading next instruction from RDATA. Data Transfer involves transferring data from memory to register (MOVA and MOVB), reading address from memory, sending that to memory back to get the addressed data and transfering to registers (MOVAM and MOVBM) and finally writing back to memory (MOVM).
