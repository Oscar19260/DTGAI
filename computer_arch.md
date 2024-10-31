# Computer Architecture
## Models
### The Von Neumann Model
Conventional digital computers have a common form that is attributed to von Neumann.
Consists of five major components:
1. __Input Unit__: provides instructions and data to the system.
2. __Memory Unit__: store data.
3. __Arithmetic and Logic Unit (ALU)__: process the instruction and data.
4. __Control Unit__: directs the ALU to carry out processes.
5. __Output Unit__: receive the results.

<img alt="Von Neumann Model" src="/img/vonneumannmodel.jpg" 
     style="display: block; margin: 0 auto">
> The ALU and control unit are frequently referred to collectively as the Central Processing Unit (CPU).

### System Bus Model
This model patitions a computer system into 3 subunits: CPU, Memory and Input/Output (I/O).
The comunication among the components are by means of a shared pathway called __system bus__, which is made up of:
* __Data Bus__: carries the information being transmitted.
* __Address Bus__: identifies where the information is being sent.
* __Control Bus__: describes aspects of how the information is being sent, and in what manner.
* __*Power Bus__: for electrical power to the components.

<img alt="System Bus Model" src="/img/systembusmodel.jpg"
     style="display: block; margin: 0 auto">
> Some architectures may also have a separate I/O bus.

### Harvard Model
Harvard architecture refers to a memory structure in which the processor is connected to two independent memory banks via two independent sets of buses.
1. __Data Memory__: stores data, accessed by the ALU for read/write operations through distinct data addresses.
2. __Program Memory__: stores instructions, fetched by the control unit using separate instruction addresses.
3. __Control Unit__: manages the flow, sending op codes to the ALU and receiving status signals.
4. __ALU__: performs calculations and interacts with both memory units.

<img alt="Harvard Model" src="/img/harvard.gif"
     style="display: block; margin: 0 auto">
> Instructions and data are handled independently, allowing simultaneous access and improving efficiency.
> This model is faster than Von Neumann model, but more expensive. 
