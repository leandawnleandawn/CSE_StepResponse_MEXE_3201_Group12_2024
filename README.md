# Laboratory 2: Step Response 

## Objective: 
  To use MATLAB as a tool to simulate the step response of the following transfer functions of the system

## Background:
### Transfer Function: 
  Imagine your system is a black box. You put something in (the input), and you get something out (the output). The transfer function, written as a fancy capital G(s), is a mathematical recipe that tells you exactly how that black box transforms the input into the output. It's like a secret formula that depends on the inner workings of the system.

  Here's the technical part: The transfer function uses Laplace transforms (don't worry, these transforms turn functions of time into functions of a variable 's'). It expresses the output (Y(s)) as a fraction of the input (X(s)) based on the system's properties.
### Step Response: 
  This is where things get interesting for your lab. The step response is what happens to the output (y(t)) when you give the system a very specific input: a sudden jump from zero to a constant value (like flipping a light switch on). It's like a test question for your system, revealing how it reacts to a quick change.

  By analyzing the step response (a graph of y(t) vs. time), you can learn a lot about the system. Does it reach the final output value quickly? Does it oscillate before settling? The shape of the curve tells you things like the system's stability, speed, and accuracy.

### _Why are they important in your lab?_

By understanding the transfer function (the recipe) and observing the step response (the result), you can:

**Predict system behavior:** You can use the transfer function to anticipate how the system will react to different inputs, not just a step change.
**Diagnose problems:** A wonky step response can indicate issues with your system's components.
**Tune and improve the system:** By analyzing the step response, you can see how to adjust the system to get the desired output.

## Procedure:
1. Define the following transfer functions in MATLAB using the tf function or by specifying the numerator and denominator coefficients.
2. Plot the step responses using the step function.
3. Then use simulink to plot the step responses. Also apply sinusoidal source and compare the response.

## Results

### Second Order Underdamped System
  Represents the underdamped system
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/c3b88b35-f6a4-4a51-8ea0-13a5a88cb7ad)
  2. Simulink
     - Step Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/143849f7-16b9-4735-ad5d-6ac562c6f229)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/13be6ba2-3bd1-49db-9e0a-37d94e0383c2)

### Second Order Overdamped System
  Represents the overdamped system
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/95395cb9-e0d4-4f22-8756-312daca8e9ba)
  2. Simulink
     - Step Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/65953a7b-15c5-44f9-abc1-e3f448391293)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/35888cb2-3318-4867-b69f-09a325d965dd)

### Second Order Critically Damped System
  Represents a critically damped system
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/e6e0f400-e8fa-493f-a82b-6c5b77d59ce4)
  2. Simulink
     - Step Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/65953a7b-15c5-44f9-abc1-e3f448391293)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/35888cb2-3318-4867-b69f-09a325d965dd)

### First Order System
  Represents a first order system
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/75079fd3-06a5-4dab-a784-7ef886bf1731)
  2. Simulink
     - Step Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/f8d44d61-a139-4168-88db-226c7a6d5ef1)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/4d661294-b6dc-4405-9689-a499508aba0d)
       
### Resonant System
  Modeling a resonant system with a sharp peak
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/0a47eb34-b027-4aec-9925-28efeb8e6cc1)
  2. Simulink
     - Step Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/77c84b3a-9c6f-4e6c-94c8-121ee2657026)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/f2810f49-ec47-4b46-9895-717ff2213163)

### Electrical Filter with Multiple Poles
  Modeling of electrical filter with multiple poles
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/b05e2d47-c791-44ef-87e6-ece890ed4d32)
  2. Simulink
     - Step Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/4d512bf1-9df1-4364-9ae7-46104cadfc1b)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/7d48674d-69b9-4967-b601-f50b83713dab)

### Plant with Time Delay
  Modeling a system with Time Delay
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/f5f1ad97-2eba-4a68-a7a7-1ce0e6889f7d)
  2. Simulink
     - Step Response
      ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/0bf625ec-05f3-4164-a634-4206208efce4)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/4c14b702-5d7b-49db-acf4-7a5aedc1ecdb)

### Nonlinear System Approximation
  Modeling a nonlinear system with a polynomial approximation
  1. MATLAB Step Response
  ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/95192f6a-a91f-4b8d-8761-e571790164f3)
  2. Simulink
     - Step Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/e753abc3-9b17-4d03-b9ad-4ee8e1bf0778)
     - Sinsodial Response
       ![image](https://github.com/leandawnleandawn/CSE_StepResponse_MEXE_3201_Group12_2024/assets/83767299/474658e4-3284-4c47-bfd6-f6934eaeeed5)

