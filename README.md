
### Assembler Project 
###
### Final project - System Programming Laboratory course - The Open University - Israel
### Written in C
### 
### Authors: Gal Pinto, Ben Kalamaro
### Date: 13.08.2022

###

##### Mainly the project is about creating an assembly program using C
##### The program takes a *.as file as an input, filled with Assembly code
##### Processes it-> translates the assembly to binary and then to special predefined base32
#####  Outputs:
 * .am -> pre-processed file, if macros were found at the source
 * .ob -> base 32 code translation
 * .ent -> entries labels table(if exists)
 * .ext -> external labels table(if exists) 
The syntax of the assembly and its constraints are specified in the attached project instructions

#### Project Contents:
#####  assembler:
 * global.h - global header - globals, macros, and typedefs
 * assembler.c/.h - main program
 * utils.c/.h - utility functions
 * macro_reader.c/.h - pre-process functions
 * first_pass.c/.h - first pass functions
 * second_pass.c/.h - second pass functions
 * ins_analyzer.c/.h - instruction commands analyzer and processor
 * gui_analyzer.c/.h - guidance commands analyzer and processor
 * file_writer.c/.h - write to file functions
 * text_parser.c/.h - text parsing and processing functions
 * free_memory.c/.h - memory freeing functions
 * makefile
 * *.as - tests source files
#####  Tests:
###### In the Tests directory you can find:
 * Tests-ReadMe.txt: a file specifies the contents of the Tests directory.
 *  errors.txt: a text file that specifies all the known errors in our program
######  f_test: failed tests
 *  .txt files explaining what errors you will get when running the file
 *  .png a screenshot of the terminal running the program
######  s_test_output: successful tests expected output files
 *  expected_am - expected .am output file for comparison
 *  expected_ent - expected .ent output file for comparison
 *  expected_ext - expected .ext output file for comparison
 *  expected_ob - expected .ob output file for comparison
 *  .png - a screenshot of the terminal running the program

##### How to run a Test:
 pass the test file's name, as an argument in CLI when running the program, without its extension.<br />
 the file must have .as extension.<br />
Example:<br />
On terminal:<br />
`.../workspace/assembler: ./assembler s_test_1`<br />
You can also run several tests in one command:<br />
`.../workspace/assembler: ./assembler s_test_1 s_test_2 f_pass_fail_1 f_pass_fail_2 f_pass_fail_3 s_pass_fail_1`
