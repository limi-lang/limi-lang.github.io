# Rationale
<!--- 

Plan
- Software problems are systemic and incremental solutions are not enough to solve the problems that exist.
- An integrated holistic, full stack system that fully models every problem is required. Can we design a universal software/tool/language that fully solves the problems that every software abstraction ever created solves.
- Software is never finished
- The current architecuture of the software stack
 -- OS
 -- Language
 -- Persistent storage
 -- Network access
 -- GUI
- Software problems are interlinked
- A software textual language that models persistent storage access and free variables as interfaces to the external world. (Non deterministic functions are equivalent to free variables so getting data from persistent storage is the same as getting it from the environment through free variables)


- The author argues that a language that provides a consistent abstraction for persistent storage and uses free variables as interfaces to the external world is enough to solve all many dependency and interface problems that exist today.

- seemingly very small restrictions in programming languages create the software paradigms.
- control imposed upon direct transfer of control.
- control imposed upon indirect transfer of control
- restriction of mutation of variables

We continually create new abstractions and write more code to solve existing problems

Software systems are very sensitive to software interfaces.

Can we create a software language that fully models

Textual Computer languages have evolved to become the main and most powerful ways of instructing computers' 

Security and software complexity are systemic problems endemic to the software industry today. They exist due to the architecture of the tools and processes used to design software systems. These problems are tied to historical decisions and developments previously made in the industry. Even when newer and better systems exist, it is often hard to kill off the old systems.
It is hard to kill off poorly specified and designed systems.

The earliest development progress was about providing as much functionality as possible. 'hacking everything together and making it work'

Is there a system that can correctly and mathematically abstract all the functionality of all the software systems. The software interfaces  that exist today are tied to the incompleteness of abstractions. (e.g web programs are tied to client server model )

Unfinished software is a software interface problem. Ever growing software code bases. 

It  is not always clear where software interfaces should be. 

Zero day vulnerabilities are exist in almost every production software system in use today.
These are systemic problems endemic to the software industry.

Is it possible to design a software development processs that guarantees zero bugs.

Semantic additions that limi makes
- transfer of control is a low level abstraction, should be separated from programming languages specification. Imposition of transfer of control should be left to the interpreter/ compiler so that they can eke out every performance gain for the chosen target machine. Transfer of control is target machine specific
- Exclusively use free variables a software interfaces between software modules and the external world.
- Provide a network agnostic universal persistent storage mechanism
--->


Software systems currently have systemic problems. These problems are endemic to the industry and exist due to the architecture of the tools and processes used to design software systems.
These problems include; 

- Software Security
- Software Complexity
- Software Compartibility / Interoperability
- Dependency Hell
- Abstraction Hell
- State Management
- Software bloat and duplication
- Technical debt
- Poor abstractions / Abstraction abuse
- Losing the forest for the trees
- Change fatigue
- Obsolescence
- Failure to separate concerns
- Backwards compartibility
- Abstraction leakage ( control transfer is a low level concern)
- Lost productivity in learning exercises
- Smallest unit of production code

<!---
Needs a mathematically modelled solution. Access to IO, Process Modelling
Some solutions are bolten on
Software errors are very expensive. ( Solution Mathematical rigor ), we should treat  a software package as rigorously as a mathematical theorem

Limi is a multi-paradigm programming system. It is more than a language. 
Mathematicians admit that there is no known solution to an open problem. Business people make it work

Solution
Holistic abstractions

Glossary
Accidental investigation techniques
Safety critical applications
--->