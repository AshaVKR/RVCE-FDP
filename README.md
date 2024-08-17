
Design of a Processor
step1: Write an application using C  code, compile using GCC compiler(linux), measure an output O0

step2: Every Processor has got an architecture. We are going to model that architecture spec in C, then run the application on the obtained model to measure an output O1. Architecture defines different instruction format. we need to check O0 == O1

step3: we make a soft copy of the hardware using High Level Language and use a converter to convert the high level language to verilog code. Verilog code of an architecture is called Micro Architecture.From step3 measures an output and check O2==O1.

We divide the top verilog code into Processors and Peripherals/IPs. Processor will not run automatically ,Processor needs peripherals to run. We make sure Processor is a sythesizable Processor. Synthesizable means each and every line of the Processor should be able to convert to gates. Peripherals are again divided into Macros(synthesizable RTL) and Analog IPs are built using circuits(NMOS,PMOS)(functional RTL) We do Synthesis, Placement, Routing and Power Planning in this stage and we generate a file called GDSII. After this it will go to some digital level checks(it basically checks for connectivity ) and this goes to foundary and once we get from factory we have to create a board and we pass the same test bench in C language and measures and Output O4 and check O4

![image](https://github.com/user-attachments/assets/565d8c0e-4770-43f6-b3d3-68209860198f)

![image](https://github.com/user-attachments/assets/d080435d-072b-4c6f-940a-1cee4c9594fe)

![image](https://github.com/user-attachments/assets/28e33b48-8eec-4be2-909f-fa0fc56e3c81)








  


