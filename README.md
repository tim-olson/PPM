# PPM
Contains FAQ information and example Parametric Part Modeling (PPM) scripts for TurboCAD.  

1. Script Format:  

// File: <Name>.ppm  
// Description: <Short plain‑English summary of what this PPM creates>  
// Author: <Your Name>  
// Date: <YYYY‑MM‑DD>  
// Notes:  
//   • Dependencies: Macro\<Helper>.ppm (if any)  
// Confirmed: +0 increment this value when tested  

You must provide inline documentation such that the AI will learn the process of  the  script.  
Use a descriptive file name to allow the AI identify your script context

2. FAQ Format:  
One FAQ per text file.  If you are extending or modifying an existing FAQ, add your name to the Modified section.  

Author:  
Provide your name for citations.  
Modified:  
Name and modification reason.  
Question:  
Provide your detailed question.  
Answer:  
Provide your detailed response to the question.  

3. Misc Folder  
A "reference guide" that gets updated by the AI based on content in the PPM repository using the following prompt:  
 
Instruction: Create a TurboCAD Parametric Parts Modeling (PPM) Quick Reference Guide.  
The guide should be multi-page (6–8 pages), beginner-friendly, and organized by categories of functions.  
Include these sections:  
Script Basics  
Syntax rules, comments (//), identifiers, reserved words.  
Parameters (Parameter()) with examples for LINEAR, ANGULAR, TEXT, COLOR, MATERIAL, CHECKBOX.  
Input/Output usage.  
Units (Units(1[in]), Units(1[mm])).  
RefPoint for placement.  
2D Geometry Functions  
Circle, Rectangle, Polyline, Arc0/Arc1, Fillet.  
Example of a rectangle with rounded corners.  
3D Creation Functions  
Thickness, Sweep, Sphere, Cone, Box (custom function).  
Examples of a simple 3D box and a sweep.  
3D Boolean Operations  
BooleanUnion, BooleanSubtract, BooleanIntersect.  
Example of subtracting a cylinder from a sphere.  
3D Modification Functions  
G3Fillet, G3Chamfer, G3Offset, G3Shell, G3Bend.  
Include simple examples for each.  
Transformations  
Move, RotateX/Y/Z, optional scale/shear if supported.  
Example of rotating a circle and moving it.  
SetProperties() (Styling & Attributes)  
PenColor, PenWidth, Brush, Material, Solid toggle.  
AUX properties (e.g., #$AUX@_Contour).  
Example with different styled boxes.  
Text Functions  
Text, TextFont, TextStyle.  
Example of bold, italic, rotated text.  
Math & Logic Helpers  
IF, min(), max(), Mod(), Div(), Array().  
Example of IF condition with Rectangle(L,H) vs Rectangle(H,L).  
Grouping & Symbols  
Group().  
StaticSymbol(), FolderList().  
Custom functions via Macro folder.  
Formatting requirements:  
Use section headers per category (one per page where possible).  
Use tables for quick lookup of functions, arguments, and purpose.  
Provide short runnable code snippets under each function.  
Highlight reserved keywords clearly.  
Keep it concise but readable (6–8 pages).  
Design it as a quick reference (not a full tutorial).  
