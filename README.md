# Automated RTL Testbench ( ART )

## Introduction 

![image](https://user-images.githubusercontent.com/82292548/181595137-640a89d9-30f7-402b-b3ae-74e779638404.png)


### ART is an EDA software tool that was developed by a group of EECE2023 students :  
###### - Aya Reda 
###### - Sohila Akram 
###### - Abdullah Said 
###### - Abd-El-Rahman Sabry
###### - Abd-El-Aziz Mohamed Gamal-El-Deen
###### - Abd-El-Rahman Mohamed Nour-El-Deen



<br>
<br>
<br>
<br>

  The project aims to change the traditional way of developing RTL and testing its functionality, The software has three main stages Resources , Design-Test GUI and Output Stage you can also watch this bref [video about the software ](https://drive.google.com/file/d/1bkmGFnX-tNFf6AMr_Rgmt7jzRNeUYhQX/view?usp=sharing) 
  
  ![image](https://user-images.githubusercontent.com/82292548/181595721-9b931376-ae1b-4283-b709-a3e02b270712.png)
<br>
<br>
<br>
## Resources Stage

The resources stage is the verilog HDL design files for the next GUI stage.
there are 3 main sources for verilog files in the software 

<br>
<br>
<br>

## Standard library 

The standard library is used to generate various configurable synthesizable verilog files to be used in your design. For example: if you want to build a processor you will find memories, ALUs, Pipes ...etc 

<br>
<br>
<br>

## External Verilog Files 

You can write a verilog file yourself, then import it into the design GUI.

<br>
<br>
<br>

## Finite State Machines 

The software allows you to draw the state diagram and it will generate the verilog file for the FSM [still under development].

<br>
<br>
<br>

## Design Test GUI Stage

You can use the files from the resources stage, define the inputs and outputs and connect them to build a schematic of your digital design blocks.
The tool then will generate all the required verilog files (ex: top_module.v)
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

We can easily generate all the test vectors using ATSL. ART Testing Scripting Language or ATSL is a simple scripting language that is only used for the purpose of describing the input/output relationship for easier testing. It has alot of built-in functions that will make it easier like (carry) in following example and others like (rand) that is used to generate a random testcases for a given range.

|![image](https://user-images.githubusercontent.com/82292548/183482442-ddeac318-cbaa-4222-8e52-00b14bd61c27.png)|
|:--:|
| The combinational test|

|![image](https://user-images.githubusercontent.com/82292548/183484365-d115efab-d835-4a90-9555-2d061bc0511b.png)|
|:--:|
| The generated testcases|

|![image](https://user-images.githubusercontent.com/82292548/183485058-ec3bd0db-5fae-415f-9d2b-2f02acd9a8ca.png)|
|:--:|
| The generated testcases|


<br>
<br>
<br>

### Sequenctial Testing 

<br>
In sequential testing we can specify a relationship as out[i+1]=out[i]+1 and check if every out is equal to the previous value plus one.
<br>

|![Slide3](https://user-images.githubusercontent.com/82292548/183480640-9c386281-7fca-482a-b9d3-04b7a4c30b4b.PNG)|
|:--:|
| The sequential test|


<br>
<br>
<br>

# Updated Vesion of ART

## Install ART

`git clone https://github.com/Digital-Geeks-23/ART-GP.git`

## Required Library

`pip install Pyqt5`


## Run ART

`python ART.py`



# New ART Layout
https://user-images.githubusercontent.com/102327986/191865241-ac60b5d9-5de1-4b7f-b93b-8eb464a9d793.mp4



## Cellview
https://user-images.githubusercontent.com/102327986/191864431-2454dd88-1ca7-49f0-849b-2cd6e63b3c0d.mp4



## Hierarchy
https://user-images.githubusercontent.com/102327986/191864525-70f794fc-dcc0-4e51-8706-50a8abf48c60.mp4



## Inspector
https://user-images.githubusercontent.com/102327986/191864548-ae19ca9b-59c5-4b9e-bfb2-bda56ba4dc34.mp4



## Command line
https://user-images.githubusercontent.com/102327986/191864489-65b487ad-061f-44ee-b63b-dc780900bd3b.mp4


However long and complex tests you need to apply for your design, ART will help you save time, stop doing boring systematic stuff. Just write simple expressions or even the expected outputs at some given input and the testbench file will be generated for you in a blink.
