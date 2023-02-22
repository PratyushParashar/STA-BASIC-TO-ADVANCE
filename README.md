# STA-BASIC-TO-ADVANCE

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


Question 3-What is the difference between ‘simple_max.lib’ and ‘simple_min.lib’.

Answer-Comparing simple max.lib with simple min.lib, it can be seen that both files have different values for parameters like delay, fall transition, cell rise, rise transition, cell fall, etc. The maximum value for each parameter is defined in the simple max.lib file, while the minimum value is defined in the simple min.lib file.

## DAY3
<img width="678" alt="day 31" src="https://user-images.githubusercontent.com/126072954/220636701-d40b8985-dc8a-4ac2-9ea7-6fb605756c3a.png">



QUESTION -Change the number of paths being reported to 100
                • report_checks –from F1/CK -endpoint_count 100
                
                
<img width="476" alt="31" src="https://user-images.githubusercontent.com/126072954/220637296-1ce6b1fb-df44-4317-9311-8cf37a4a9037.png">



  Analyze each path in detail and understand
  
  
  <img width="448" alt="PATHS" src="https://user-images.githubusercontent.com/126072954/220644244-cdca7eb6-c38e-462e-863c-7e9e47dadf88.png">

PATH 1-
  
  
<img width="709" alt="PATH 1" src="https://user-images.githubusercontent.com/126072954/220644341-373f1d07-f94c-4d8b-b426-fb70a1cdfc3d.png">

PATH 2-
   
   
<img width="678" alt="PATH 2" src="https://user-images.githubusercontent.com/126072954/220644434-6a641fe7-38fd-40b1-975c-776e8cc05bac.png">
    
PATH 3- 
    
    
<img width="678" alt="PATH3" src="https://user-images.githubusercontent.com/126072954/220644641-bfdec109-e525-429c-b908-3360ea9dd191.png">
    
PATH 4-
    
    
<img width="678" alt="PATH 4" src="https://user-images.githubusercontent.com/126072954/220645977-2130889f-70fc-4e10-932b-41777c6bc402.png">
    
PATH 5-
    
    
<img width="678" alt="PATH 5" src="https://user-images.githubusercontent.com/126072954/220646255-702ec4ed-5344-404b-b273-75a718f1d0b9.png">
    
PATH 6- 
    
    
<img width="678" alt="PATH 6" src="https://user-images.githubusercontent.com/126072954/220646394-3a7a4ffa-d225-4a6b-a56f-b8552e5e2867.png">
    
PATH 7-
    
    
<img width="1176" alt="PATH 7" src="https://user-images.githubusercontent.com/126072954/220646487-bc813913-7616-4775-8e6e-9e1bf0513af1.png">
     
PATH 8-
    
    
<img width="710" alt="PATH8" src="https://user-images.githubusercontent.com/126072954/220646572-35c4bc0f-299e-4497-beba-f5c4f58852fe.png">

## INFERENCE- OBSERVED ON ALL THE PATHS THE SLACKS WERE VIOLTED


## DAY- 4
COMMAND FOR GETTING INTO DAY 4 LAB


<img width="643" alt="day4" src="https://user-images.githubusercontent.com/126072954/220656715-be0808e9-beb0-41d6-87b5-914eee2a7fd0.png">


<img width="323" alt="day4a" src="https://user-images.githubusercontent.com/126072954/220656801-f4b392e3-0101-471f-b3a0-fc855e21c787.png">


SLACK ON CLOCK GATING PATH

<img width="746" alt="day41" src="https://user-images.githubusercontent.com/126072954/220657124-5cccdf89-e7f1-4f45-afbb-c5b6b36eee2a.png">

<img width="553" alt="day41a" src="https://user-images.githubusercontent.com/126072954/220657232-d5eab1ed-2f6e-44ba-a242-158489602f4d.png">

<img width="522" alt="day41b" src="https://user-images.githubusercontent.com/126072954/220657314-3a60540c-64a5-47ba-be95-37c441d988d8.png">

## SLACK IS VIOLETED 

##  ASYNCH PIN CHECK


<img width="640" alt="44" src="https://user-images.githubusercontent.com/126072954/220659298-8b3a9e7c-80cb-4d76-be72-c977e3d4611d.png">

<img width="330" alt="44A" src="https://user-images.githubusercontent.com/126072954/220659645-7f134d04-3f71-4ac8-a11b-d9aa327da852.png">

COMMAND-

<img width="625" alt="44B" src="https://user-images.githubusercontent.com/126072954/220661146-6d051785-8bab-4160-bb33-a2f95ceb79f9.png">



<img width="444" alt="44C" src="https://user-images.githubusercontent.com/126072954/220661185-59b07325-3c5e-4064-93c0-a889dcd4384f.png">

## SLACK HAS BEEN MET

## DAY 5-













