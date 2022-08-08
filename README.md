# Automated RTL Testbench ( ART )

## Introduction 

![image](https://user-images.githubusercontent.com/82292548/181595137-640a89d9-30f7-402b-b3ae-74e779638404.png)


### ART is an EDA software tool that was developed by a group of EECE2023 students :  
###### - Aya Reda 
###### - Sohila Akram 
###### - Abd-El-Rahman Sabry 
###### - Abd-El-Rahman Mohamed Nour-El-Deen
###### - Abd-El-Aziz Mohamed Gamal-El-Deen
###### - Abdullah Said 

<br>
<br>
<br>
<br>

  The project aims to change the traditional way of developing RTL and testing its functionality, The software has three main stages Resources , Design-Test GUI and Output Stage you can also watch this bref [video about the software ](https://drive.google.com/file/d/16u4fu3__i1OCJmS3Fb07G-D56OvBuErb/view) 
  
  ![image](https://user-images.githubusercontent.com/82292548/181595721-9b931376-ae1b-4283-b709-a3e02b270712.png)
<br>
<br>
<br>
## Resources Stage

The resources stage is the verilog files source for our design in the next gui stage.
there are 3 main sources for verilog files in the software 

<br>
<br>
<br>

## Standard library 

The standard library is used to generate verious configurable verilog files to be used in your design. For example: if you want to build a processor you will find memories, ALUs, Pipes ...etc 

<br>
<br>
<br>

## External Verilog Files 

you can write a verilog file by yourself and then import the file into the design 

<br>
<br>
<br>

## Finite State Machines 

The software allows you to draw the state diagram and it will generate the verilog file for the FSM but it still under development.

<br>
<br>
<br>

## Design Test GUI Stage

You can use the files from the resources stage and by defining the inputs and outputs you can use them to build a schematic of your design and the tool will generate all the required verilog files.
<br>
*if the whole design is based on the std lib it will be always synthesizable*

<br>
<br>
<br>
  
|![image](https://user-images.githubusercontent.com/82292548/181603685-08c264db-07bb-460c-a35d-03c2ed07e4bc.png)|
|:--:|
| One Cycle MIPS |

<br>
<br>

|![image](https://user-images.githubusercontent.com/82292548/181862894-8c063966-4a06-4fce-96a2-9486dbcb94fd.png)|
|:--:|
| UART Transmitter |

<br>
<br>

|![image](https://user-images.githubusercontent.com/82292548/181863107-24f03090-1dd9-4065-9c09-b74b421e9dcc.png)|
|:--:|
| Four Bit adder |

<br>
<br>
<br>

## Testing

We can say The Testing in ART has an analogy with control systems 

|![image](https://user-images.githubusercontent.com/82292548/181863279-b9dd2569-4080-403c-b346-d1d54566e1a8.png)|
|:--:|
| Four Bit Adder Under Test|

<br>
<br>
<br>

### Combinational Testing 
<br>

for example if i want to test a combinational circuit 

<br>
<br>
<br>

|![Slide1](https://user-images.githubusercontent.com/82292548/183480438-f961ecef-bcbb-4a97-86cb-5cc8f8dcb21a.PNG)|
|:--:|
| The combinational test|

We can easily generate all the test vectors using ATSL (ART Testing Scripting Language) script which is a simple scripting language that is only used for the purpose of discribing the in out relationship and it has alot of built-in functions that will make it easier like (carry) in following example and others like (rand) that is used to generate a random testcases in a given range 

|![image](https://user-images.githubusercontent.com/82292548/183482442-ddeac318-cbaa-4222-8e52-00b14bd61c27.png)|
|:--:|
| The combinational test|

<br>
<br>
<br>

|![Slide3](https://user-images.githubusercontent.com/82292548/183480640-9c386281-7fca-482a-b9d3-04b7a4c30b4b.PNG)|
|:--:|
| The sequential test|

