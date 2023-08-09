# Theory:

Counter is a type of circuit, which counts or which can be used for counting purposes. Or counting is such a digital device, which counts clock pulses in binary. Counter is a sequential logic circuits composed via wiring together flip-flops, which are used to count binary pulses being applied on these flip-flops. When a clock pulses are applied on input of some counter, the flip-flops present inside the counter change its state in such a way that stored binary number on it reveals the number of input pulses passing through it.

There are two types of counters in digital logic circuit that are used to count the numbers of bits and these types depends upon the clock pulse applied to the flip flops.

- Asynchronous Counter (Ripple Counter)

These are the counters in which we do not use universal clock, main clock is only applied to the first flip flop and then for rest of flip flops the output of previous flip flop is taken as a clock.

- Synchronous Counter

These are the counters in which we use a universal clock that is common to all flip flops. 

## Ripple (Asynchronous Counter)

To design a ripple counter, we should first design a J-K Flip Flop. To design a J-K flip flop, we have to first design a 3 input NAND gate and a LATCH. We have designed 3 input NAND gate and LATCH as below and packaged them into components.

    
<center>
<img src="./images/E8p1.png" style="width:50%">

##### 3-IN-NAND (27, 28, 29: inputs. 30: Output)  		
</center>




<center>
<img src="./images/E8p2.png" style="width:50%">

##### LATCH
</center>



Using the 3-In-NAND and LATCH, we have designed J-K-FlipFlop as below. Then packaged it into component.
<center>
<img src="./images/E8p3.png" style="width:50%">

##### J-K-FlipFLop (83, 84: Inputs. 85, 86: Outputs)
</center>



Now using the J-K-FlipFLop, we have designed the ripple counter as below.

## 3 Bit Ripple Counter
***LSB: 191 MSB: 193***

### Clock 1: 
<center>
<img src="./images/E8p4.png" style="width:50%">

##### Number: 000
</center>



### Clock 2:

<center>
<img src="./images/E8p5.png" style="width:50%">

##### Number: 001
</center>

### Clock 3:

<center>
<img src="./images/E8p6.png" style="width:50%">

##### Number: 010
</center>

### Clock 4:

<center>
<img src="./images/E8p7.png" style="width:50%">

##### Number: 011
</center>

### Clock 5:

<center>
<img src="./images/E8p8.png" style="width:50%">

##### Number: 100
</center>

### Clock 6:

<center>
<img src="./images/E8p9.png" style="width:50%">

##### Number: 101
</center>

### Clock 7:

<center>
<img src="./images/E8p10.png" style="width:50%">

##### Number: 110
</center>


### Clock 8:

<center>
<img src="./images/E8p11.png" style="width:50%">

##### Number: 111
</center>

### Clock 9: (Back to initial state)


<center>
<img src="./images/E8p12.png" style="width:50%">

##### Number: 000
</center>


## 3-Bit synchronous Counter

Using J-K-FlipFlop and AND gate we can design asynchronous counters as below.

***204: LSB, 206: MSB***

### Clock 1:

<center>
<img src="./images/E8p13.png" style="width:50%">

##### Number: 111
</center>

### Clock 2:

<center>
<img src="./images/E8p14.png" style="width:50%">

##### Number: 110
</center>

### Clock 3:

<center>
<img src="./images/E8p15.png" style="width:50%">

##### Number: 101
</center>

### Clock 4:

<center>
<img src="./images/E8p16.png" style="width:50%">

##### Number: 100
</center>

### Clock 5:

<center>
<img src="./images/E8p17.png" style="width:50%">

##### Number: 011
</center>

### Clock 6:

<center>
<img src="./images/E8p18.png" style="width:50%">

##### Number: 010
</center>

### Clock 7:

<center>
<img src="./images/E8p19.png" style="width:50%">

##### Number: 001
</center>

### Clock 8:

<center>
<img src="./images/E8p20.png" style="width:50%">

##### Number: 000
</center>

### Clock 9: (Back to initial state)

<center>
<img src="./images/E8p21.png" style="width:50%">

##### Number: 111
</center>
