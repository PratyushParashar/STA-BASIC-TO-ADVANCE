# STA-BASIC-TO-ADVANCE

<img width="640" alt="front" src="https://user-images.githubusercontent.com/126072954/220913033-93c81323-bea4-467f-80d7-6a7da1cce694.png">


TABLE OF CONTENTS


1- DAY1- INRTODUCTION AND BASICS OF STA


2- DAY2- LIBERTY FILE AND SPEF FILE


3- DAY3- SLACK COMPUTATION


4- DAY4- CLOCK GATING CHECK AND ASYNCH PIN CHECK


5- DAY5- CPPR AND ECO INSERTION


## DAY1 
CONTENTS OF STANDARD CELL


<img width="768" alt="STANDARD CELL" src="https://user-images.githubusercontent.com/126072954/220616224-98b42008-01d3-4185-8bbf-29e9ffedd95d.png">

SKY 130 LIBRARY



<img width="336" alt="SKY130" src="https://user-images.githubusercontent.com/126072954/220616821-541c4b3d-a0e5-477f-a24c-51c0599fa375.png">

NAND GATE


<img width="254" alt="NAND" src="https://user-images.githubusercontent.com/126072954/220617319-b1e89dc5-54d4-4a4b-ad5b-7735c25df93f.png">




DESIGN CONTRAINT AND TIMING CONSTRAINT


COMMAND-

<img width="738" alt="CONSTAINT COMM" src="https://user-images.githubusercontent.com/126072954/220619795-7eeadce7-ad7f-4b6e-a82f-6061df86cfc2.png">




<img width="836" alt="constrain file" src="https://user-images.githubusercontent.com/126072954/220617487-0e070726-f770-47c8-8afa-04bca6285634.png">






INPUT PINS AND OUTPUT PINS



<img width="573" alt="INPOUP" src="https://user-images.githubusercontent.com/126072954/220618215-f60cf4fa-68ba-4bba-8661-048084811401.png">



RUN OpenSTA
COMMAND-


<img width="718" alt="OPENSTA COMM" src="https://user-images.githubusercontent.com/126072954/220619030-933f164a-0a57-43be-9ae1-d094ef6018ca.png">
FILE-


<img width="388" alt="OPENSTA" src="https://user-images.githubusercontent.com/126072954/220618661-658c077d-8274-4c87-864a-529dc5691426.png">






## DAY 2

Question 1-Find all the cells in simple_max.lib

COUNT-

<img width="848" alt="21" src="https://user-images.githubusercontent.com/126072954/220623708-70282287-1eed-4796-958d-81bdd62adf07.png">

CELLS-



<img width="718" alt="1" src="https://user-images.githubusercontent.com/126072954/220625719-08918714-0eff-4373-aede-ce61df5db1fd.png">
<img width="718" alt="2" src="https://user-images.githubusercontent.com/126072954/220626033-8ca6b96c-d841-4ab1-bab1-cd478a8fe9b8.png">
<img width="718" alt="3" src="https://user-images.githubusercontent.com/126072954/220626293-dc33724b-9d77-4b2f-a1b1-a857eb754a46.png">
<img width="718" alt="4" src="https://user-images.githubusercontent.com/126072954/220626562-37db7867-ee03-4797-a1d9-33e772413730.png">
<img width="718" alt="5" src="https://user-images.githubusercontent.com/126072954/220626915-f99b2c70-bc08-4e2d-9057-e5c7b0f9c372.png">


Question 2- Find all the pins of the cell NAND2_X1 in simple_max.lib


<img width="321" alt="QUE2" src="https://user-images.githubusercontent.com/126072954/220630731-51686c60-2d51-4a77-90a0-06450e3dedf5.png">


Question 3-What difference you see between NAND2_X1 and NAND3_X1



<img width="336" alt="DIFFRENCE" src="https://user-images.githubusercontent.com/126072954/220633392-33c1de47-b05b-4d52-83b6-984553715a63.png">


Question 4-What is the difference between ‘simple_max.lib’ and ‘simple_min.lib’.

Answer-Comparing simple max.lib with simple min.lib, it can be seen that both files have different values for parameters like delay, fall transition, cell rise, rise transition, cell fall, etc. The maximum value for each parameter is defined in the simple max.lib file, while the minimum value is defined in the simple min.lib file.

## DAY3
<img width="678" alt="day 31" src="https://user-images.githubusercontent.com/126072954/220636701-d40b8985-dc8a-4ac2-9ea7-6fb605756c3a.png">



QUESTION -Change the number of paths being reported to 100
                • report_checks –from F1/CK -endpoint_count 100
                
                
<img width="476" alt="31" src="https://user-images.githubusercontent.com/126072954/220637296-1ce6b1fb-df44-4317-9311-8cf37a4a9037.png">


Analyze each path in detail and understand
  
  
<img width="448" alt="PATHS" src="https://user-images.githubusercontent.com/126072954/220644244-cdca7eb6-c38e-462e-863c-7e9e47dadf88.png">

### PATH 1 - 
F1  - CK - U6 - U4 - U5   -  A1 - U7  - A2 - F2 - D
  
  
<img width="709" alt="PATH 1" src="https://user-images.githubusercontent.com/126072954/220885845-bbcfdef8-3789-4eca-8eae-f930072faa1b.png">


### PATH 2 -

F1  -   CK -  U3  -   U5  -  A1  -  U7 -   A2 -  F2  -   D
   
   
<img width="678" alt="PATH 2" src="https://user-images.githubusercontent.com/126072954/220885912-15e1349d-785f-4398-b733-1e9140c20599.png">

    
### PATH 3-

F1  - CK  -  U3  -   U4  -  U6  -   A2  -  U7  - A1
    
    
<img width="678" alt="PATH3" src="https://user-images.githubusercontent.com/126072954/220885967-ff7fad51-86be-403f-8f02-b74cce74495e.png">

    
### PATH 4-

F1  -   CK -   U6 -  A1 -  U7  -  A1 -   F2   -   D
    
    
<img width="678" alt="PATH 4" src="https://user-images.githubusercontent.com/126072954/220886014-84556bcf-c2b0-4af0-9634-be3a1f621ad4.png">

    
### PATH 5-

F1    -   CK -  U3 -  U5   -   A2 - U7  -   A2 - F2 -  D

<img width="678" alt="PATH 5" src="https://user-images.githubusercontent.com/126072954/220886108-32317baf-8218-48b6-bd5d-e6e552e2d53a.png">

    
### PATH 6- 

F1    -   CK  -   U6   -   U4    -    U5    :   A1 -    U7   -    A2 -   F2   -   D
    
<img width="678" alt="PATH 6" src="https://user-images.githubusercontent.com/126072954/220886166-4fb66787-5593-44a6-b990-dc57dc711ce0.png">
    
  
### PATH 7-

F1  -   CK  -  U3   -  U4   -   U6    -   A2   -     U7   -   A1  -   F2    -   D
    
<img width="556" alt="PATH 9" src="https://user-images.githubusercontent.com/126072954/220889111-54ead4f8-d793-4af8-9c8c-83914bb0e0dd.png">


     
### PATH 8-

F1    -   CK  -  U6  -   A1  -   U7   -   A1  -    F2   -   D
    
<img width="420" alt="PATH8" src="https://user-images.githubusercontent.com/126072954/220886311-85a14531-5871-45dc-8198-c7c109f9d26d.png">


### INFERENCE- OBSERVED ON ALL THE PATHS THE SLACKS WERE VIOLTED


## DAY- 4
COMMAND FOR GETTING INTO DAY 4 LAB


<img width="643" alt="day4" src="https://user-images.githubusercontent.com/126072954/220656715-be0808e9-beb0-41d6-87b5-914eee2a7fd0.png">


<img width="323" alt="day4a" src="https://user-images.githubusercontent.com/126072954/220656801-f4b392e3-0101-471f-b3a0-fc855e21c787.png">


SLACK ON CLOCK GATING PATH

<img width="746" alt="day41" src="https://user-images.githubusercontent.com/126072954/220657124-5cccdf89-e7f1-4f45-afbb-c5b6b36eee2a.png">

<img width="553" alt="day41a" src="https://user-images.githubusercontent.com/126072954/220657232-d5eab1ed-2f6e-44ba-a242-158489602f4d.png">

<img width="522" alt="day41b" src="https://user-images.githubusercontent.com/126072954/220890598-c75e73f2-0826-4e14-a673-455f956f8654.png">


### SLACK IS VIOLETED 

##  ASYNCH PIN CHECK


<img width="640" alt="44" src="https://user-images.githubusercontent.com/126072954/220659298-8b3a9e7c-80cb-4d76-be72-c977e3d4611d.png">

<img width="330" alt="44A" src="https://user-images.githubusercontent.com/126072954/220659645-7f134d04-3f71-4ac8-a11b-d9aa327da852.png">

COMMAND-

<img width="625" alt="44B" src="https://user-images.githubusercontent.com/126072954/220661146-6d051785-8bab-4160-bb33-a2f95ceb79f9.png">



<img width="444" alt="44C" src="https://user-images.githubusercontent.com/126072954/220661185-59b07325-3c5e-4064-93c0-a889dcd4384f.png">

## SLACK HAS BEEN MET

## DAY 5-

### CPPR-
Common Path Pessimism Removal (CPPR) is prevalent to eliminate inherent but artificial pessimism in clock paths during timing analysis. For example, applying different conditions for the common part of the launch and capture clock paths is over pessimistic. This pessimism should be removed during timing analysis so that true critical paths can then be identified. The challenge of CPPR is that the amount of pessimism to be removed is path dependent. Existing solutions fall into two categories, critical-path-based approach and exhaustive search approach. The critical-path-based approach first identifies critical paths without CPPR consideration and then re-evaluates these identified paths with CPPR. 


<img width="641" alt="LAB 5" src="https://user-images.githubusercontent.com/126072954/220892809-f91f8af8-42d7-4353-bbd4-c2ce155c995e.png">

COMMANDS FOR LAB 5

<img width="641" alt="LAB 5 A" src="https://user-images.githubusercontent.com/126072954/220893922-233cc8c1-7269-41fc-8daa-6c9c8020cdf1.png">


### TIMING REPORT BEFORE CPPR

<img width="348" alt="LAB 5 E" src="https://user-images.githubusercontent.com/126072954/220896122-ef253cd6-09c1-483e-9745-3d5c4475cd3d.png">


COMMAND - 

<img width="641" alt="LAB 5 C" src="https://user-images.githubusercontent.com/126072954/220894497-eac1ffa0-8f0d-427f-81e2-7dfd76f93810.png">

REPORT - 

<img width="354" alt="LAV 5D" src="https://user-images.githubusercontent.com/126072954/220895358-4bcd1c17-dbae-42be-86fe-f730b8514217.png">
SLACK HAS BEEN VIOLETED


### TIMING REPORT AFTER CPPR

<img width="348" alt="LAB 5F" src="https://user-images.githubusercontent.com/126072954/220897488-d74ca7bb-90d3-4c84-b3e8-62f51f8da19a.png">

<img width="501" alt="LAB 5 G" src="https://user-images.githubusercontent.com/126072954/220898270-155ff7d7-7bcf-46da-915f-2130954be0af.png">
SLACK HAS BEEN VIOLETED

### ECO- Engineering Change Order

In the ECO cycle, we perform various analysis one by one for every check which we need to close but not closed till PnR stage. There are specialized signoff tools that help us to analyze the issue and also suggest the changes we need to do in order to close the issue. The suggested change is captured in an eco file.

COMMAND-


<img width="547" alt="LAB 5 H" src="https://user-images.githubusercontent.com/126072954/220899902-22d5863b-1408-4fb6-835e-a4a627e47ceb.png">


<img width="547" alt="LAB 5 I" src="https://user-images.githubusercontent.com/126072954/220900131-c544a73d-a037-4623-a0c6-7545fef8a431.png">

QUESTION 1- Open Verilog file s27_eco.v, what differences you find compared to s27.v

COMMAND - 

<img width="558" alt="LAB 5 K" src="https://user-images.githubusercontent.com/126072954/220902545-d1b36ca1-9451-4648-b3dc-cc833116f071.png">


<img width="1138" alt="LAB 5 J" src="https://user-images.githubusercontent.com/126072954/220903188-ca47f0e0-d5e0-46bb-81a5-0a5722d3a032.png">

QUESTION 2-  Observe the change in slack values at timing report
COMMAND - 


<img width="410" alt="LAB 521" src="https://user-images.githubusercontent.com/126072954/220904599-43e4c82c-82cf-405b-9ec3-e45c5e2f91f2.png">


<img width="407" alt="LAB 522" src="https://user-images.githubusercontent.com/126072954/220904653-1099ccf7-7a8f-4d84-8520-334318585d51.png">

<img width="356" alt="LAB 5 23" src="https://user-images.githubusercontent.com/126072954/220904701-cf441302-949a-4a70-af90-2e87828f7e60.png">

<img width="558" alt="LAB 5 24" src="https://user-images.githubusercontent.com/126072954/220904744-0f2fc65e-b536-4a36-849d-5a80ecc8e1de.png">

ACKNOWLEDGEMENTS :


Kunal Ghosh, Co-founder of VLSI System Design (VSD) Corp. Pvt. Ltd.


Vikas Sachdeva, Advisor, Tech and VLSI Coach, Trainer and Innovator at vlsideepdive.

AUTHOR :
Pratyush Parashar, M.Tech in VLSI Design (2022-2024), VIT-Vellore, Vellore, Tamil Nadu-632014, INDIA.

Contact: parasharpratyush15@gmail.com












