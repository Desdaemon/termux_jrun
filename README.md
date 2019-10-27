# jrun for termux/android terminals
usage:

	jrun <source file with main method> [args]
	
prerequisites: ecj, dx.
	
A simple bash script to run Java on Android using Dalvik Virtual Machine.

At the parent folder of the main class, a bin folder will be created which contains
the generated .class and .dex files.

The .dex files can be run independently by using this command:

	dalvikvm -cp <dex file> <main class> [args]
