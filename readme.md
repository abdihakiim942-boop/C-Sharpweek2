# Chapter 3: Processing Data

## Objectives

This chapter introduces the basic concepts of processing data in C# Windows Forms applications. By the end of this chapter, I will understand how to:

* Read user input using TextBox controls.
* Declare and use variables.
* Work with different data types.
* Perform basic calculations.
* Convert and display numeric values.

## Topics

* 3.1 Reading Input with TextBox Controls
* 3.2 A First Look at Variables
* 3.3 Numeric Data Types and Variables
* 3.4 Performing Calculations
* 3.5 Inputting and Outputting Numeric Values
* 3.6 Formatting Numbers with the ToString() Method
* 3.7 Simple Exception Handling
* 3.8 Using Named Constants
* 3.9 Declaring Variables as Fields
* 3.10 Using the Math Class
* 3.11 More GUI Details
* 3.12 Using the Debugger to Locate Logic Errors

## 3.1 Reading Input with TextBox Controls

TextBox waa Windows Forms control oo u oggolaanaya user-ka inuu keyboard-ka ku geliyo xog.

Waxaa laga heli karaa qaybta Common Controls ee Toolbox-ka.

Xogta uu user-ku geliyo waxaa lagu kaydiyaa Text property-ga TextBox-ka.

string name = nameTextBox.Text;

Text property waxay xogta u kaydisaa qaab string ah.

TextBox sidoo kale waa la nadiifin karaa iyadoo la isticmaalayo:


nameTextBox.Clear();

ama:

nameTextBox.Text = string.Empty;

## 3.2 A First Look at Variables

Variable waa meel kayd ah oo ku jirta memory-ga, taas oo loo isticmaalo in lagu kaydiyo xog.

Magaca variable-ku wuxuu matalaa meeshaas memory-ga ah.

Ka hor inta aan variable la isticmaalin, waa in marka hore lagu declare gareeyaa data type.

### Syntax

DataType VariableName;

Example:

string name;
int age;

### Data Types

Data type wuxuu qeexayaa nooca xogta uu variable-ku kaydin karo.

Noocyada caanka ah waxaa ka mid ah:

* string → waxaa lagu kaydiyaa characters ama text.
* int → waxaa lagu kaydiyaa whole numbers.
* double → waxaa lagu kaydiyaa numbers ay ku jiri karaan decimal values.
* decimal → waxaa lagu kaydiyaa decimal values oo leh precision ka badan double, waxaana badanaa loo isticmaalaa xogta la xiriirta lacagaha iyo xisaabaadka.

### String Variables

String waa isku-dar characters ah.

string university = "Jamhuuriya University";

Strings waxaa sidoo kale la isku dari karaa iyadoo la isticmaalayo + operator.

Taas waxaa loo yaqaan string concatenation.

string fullName = firstName + " " + lastName;

### Variable Naming Rules

* Character-ka ugu horreeya waa inuu noqdaa letter ama _.
* Magaca variable-ku ma yeelan karo spaces.
* Reserved keywords looma isticmaali karo magac variable.
* Waa in la isticmaalaa variable names macno leh.

### Local Variables and Scope

Local variable waa variable ka tirsan method-ka lagu declare gareeyay.

Kaliya statements-ka ku jira method-kaas ayaa heli kara variable-kaas.

Scope waxaa loola jeedaa qaybta program-ka uu variable-ku ka dhex shaqayn karo ama laga geli karo.

Local variable sidoo kale waa in marka hore loo assignment gareeyaa value ka hor inta aan la isticmaalin.