This game was created by Kaloyan Penev
for Bournemouth University
BSc Games Software Engineering
Object Oriented Programming CW2

**HOW TO PLAY**
1. Download or clone the project.
2. Open file "daydreaming.exe" in the "Release/" folder.






1.Build this project:
- in C++14 or above.
AND
- in x86 mode.

To rebuild:
1. Check that you have the SDL folder in the solution directory
2. Check that you have the SDL binary files (.dll) correctly placed in the project folder.
3. Check that the project settings are correctly set to:

-VC++ Directories:
	Include directories: $(SolutionDir)SDL\include;$(IncludePath)
	Library directories: $(SolutionDir)SDL\lib\x86;$(LibraryPath)

-Linker
	-Linker Input
		Additional Dependencies: SDL2.lib;SDL2main.lib;SDL2_image.lib;SDL2_mixer.lib;SDL2_ttf.lib;%(AdditionalDependencies)
	-System
		SubSystem: Console