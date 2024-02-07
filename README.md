
<div align="center">

<h1>TWO STAGE OPAMP DESIGN</h1>
</div>


**1. Requirements** 

- Schematic and specification:


![image](https://github.com/trong420/opamp/assets/90754954/8fd49e98-8c47-4787-9df9-addd861ffc00)


![image](https://github.com/trong420/opamp/assets/90754954/acb3f305-41f7-4efd-9fd0-0b8bb9408f4f)



**2. Design** 

- Calculate Kn, Kp from library 180nm

![image](https://github.com/trong420/opamp/assets/90754954/5da188f2-56dd-42c5-b26c-97915980cff3)

*With L of PMOS and NMOS are 0.5um*

- Find W3, W4

![image](https://github.com/trong420/opamp/assets/90754954/264776f6-91b6-4fb2-bd94-4b7a94e83f8c)

- Find W1, W2

![image](https://github.com/trong420/opamp/assets/90754954/2e1dd74d-9500-4f46-ac13-cb6a548334d0)

- Find W5

![image](https://github.com/trong420/opamp/assets/90754954/336c908b-5db2-41c0-a6b1-ba3364cb4e4a)

- Find W6


![image](https://github.com/trong420/opamp/assets/90754954/4e1f430a-06e1-4610-833c-d12291a1bdc7)

- Find W7 and calculate Av, Pdiss

![image](https://github.com/trong420/opamp/assets/90754954/fb0a7dbc-b51b-4c6e-b5a6-001ccba98d59)
![image](https://github.com/trong420/opamp/assets/90754954/4a53881e-4e22-4fa3-8c8a-9251a29561f8)


- Calculate Vbias and Vout(max), Vout(min)

![image](https://github.com/trong420/opamp/assets/90754954/6f5016d0-51fb-4be6-b61d-9185b49d8ab4)
![image](https://github.com/trong420/opamp/assets/90754954/07f84aa6-1dde-48c4-bf9e-4806683e75d3)


**3. Results** 

- LTSPICE schematic:

![image](https://github.com/trong420/opamp/assets/90754954/5957e14f-97b3-4562-851d-b2453d540471)


- Simulation of Av: Vpp of Vin is 10uV, Vpp of Vout is 56.3mV => Av = 56.3mV / 10uV = 5630 V/V

![image](https://github.com/trong420/opamp/assets/90754954/6248851c-35b8-4399-b26f-641500c95a88)



- Simulation of Gain Bandwidth and Phase Margin: At 0dB have GB = 9.23MHz and PM = 180 - 112 = 68 degree

![image](https://github.com/trong420/opamp/assets/90754954/07dbe034-5ecb-4034-975e-36ba54a36e6f)


- Simulation of ICMR: Connect Vout with Vin(-) and simulate in DC mode has ICMR: -0.081V -> 0.333V

![image](https://github.com/trong420/opamp/assets/90754954/f26bf245-4a24-42a7-afca-1c4d2deb8abe)


- Simulation of Vout range: simulate with DC mode has Vout range: -0.64V -> 0.753V 

![image](https://github.com/trong420/opamp/assets/90754954/5d2b83c4-1534-4bc0-9fee-85e584110f82)

- Simulation of Slew Rate:

![image](https://github.com/trong420/opamp/assets/90754954/ce39c008-d5d1-4226-a7b1-c6c86c596c7f)

- Simulation of Power Dissipation

![image](https://github.com/trong420/opamp/assets/90754954/1dcff3d7-54e6-4059-991c-cd7579f25ffe)


**Comparision**


![image](https://github.com/trong420/opamp/assets/90754954/04ac654d-d562-4dd1-ac66-78b4fcbea929)
