---
title: Console Exit Function
parent: Iteration 2
has_children: false
---

## Console Exit Function
On application closing we certainly always need to perform a clean up. But on the case of a c# console application there is no clear way to do it. So, we have to import a function from kernel32.dll, which is SetConsoleCtrlHandler.

The system generates **CTRL_CLOSE_EVENT**, **CTRL_LOGOFF_EVENT**, and **CTRL_SHUTDOWN_EVENT** signals when the user closes the console, logs off, or shuts down the system so that the process has an opportunity to clean up before termination.

Each console process has its own list of application-defined HandlerRoutine functions that handle CTRL+C and CTRL+BREAK signals.

Initially, the handler list for each process contains only a default handler function that calls the ExitProcess function. A console process adds or removes additional handler functions by calling the SetConsoleCtrlHandler function, which does not affect the list of handler functions for other processes. When a console process receives any of the control signals, its handler functions are called on a last-registered, first-called basis until one of the handlers returns TRUE. If none of the handlers returns TRUE, the default handler is called.

For console processes, the CTRL+C and CTRL+BREAK key combinations are typically treated as signals (**CTRL_C_EVENT** and **CTRL_BREAK_EVENT**). When a console window with the keyboard focus receives CTRL+C or CTRL+BREAK, the signal is typically passed to all processes sharing that console.