BugZapper is a basic bash debugger that can serve the following purposes:
     * Specify breakpoints in the target program (guinea pig) at which to stop execution.
     * Step through the execution of a specified number of statements in the target program.
     * Allow the examination of and state changes to the target program during execution.
     * Print program source code, breakpoints, and the currently executing line number.
     * Debug without altering target program source code.

BugZapper turns the target program being debugged into its own debugger by concatenating the debugger code with the target program's source code into a separate file for execution.

BugZapper has three main sections:
     1. The driver (bugzapper)
     2. The preamble (bugzapper.pre)
     3. The debugger functions (bugzapper.fns)

BugZapper commands:
     bp [n]       -Set breakpoint at line number [n].
     bp           -List breakpoints and break condition.
     bc [string]  -Set break condition to [string].
     bc           -Clear break conditions
     cb [n]       -Clear breakpoint at line number [n].
     cb           -Clear all breakpoints.
     ds           -Display the test script and breakpoints.
     g            -Start or resume execution
     s [n]        -Execute [n] number of statements. The default is 1.
     x            -Toggle execution trace on/off.
     h, ?         -Print the help menu.
     ! [string]   -Pass [string] to the shell.
     q            -Quit.

This software is released under the GPLv2 license. Questions or comments may be directed to hoyt.harness (@) gmail.com.
