
 Repositories:
* [embedded_linux](https://github.com/hafeezkhn/programming_C/tree/main/embedded_linux)
* [linux_internals](https://github.com/hafeezkhn/programming_C/tree/main/linux_internals)


Exception in Armv8-A
- why:exception can serve as the foundation of various crash issues
- types of exception: 
        a.Interrupts: two  types FIQ and IRQ 
          -FIQ higher priority than IRQ typically -assiciated with input pins on the core
          -external HW asserts an inturrupt request line  and corrusponding inturrupt is raised when current instruction finishes execution(assuming inturrupts are enabled)

        b.Aborts:  can be generated either on 
          -failed instruction fetches (instruction aborts)
          -failed data access(data aborts)
          -they can come from external memory system
          - can be generated from MMU of the core. a os can use MMU aborts to dynamically allocate memory to applications

