
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

- Simulation of Av

![image](https://github.com/trong420/opamp/assets/90754954/6248851c-35b8-4399-b26f-641500c95a88)
![image](https://github.com/trong420/opamp/assets/90754954/5b9ba96d-5657-4f55-a983-5c644aa82fc5)


- Simulation of Gain Bandwidth and Phase Margin

![image](https://github.com/trong420/opamp/assets/90754954/07dbe034-5ecb-4034-975e-36ba54a36e6f)


- Simulation of ICMR

![image](https://github.com/trong420/opamp/assets/90754954/f26bf245-4a24-42a7-afca-1c4d2deb8abe)


- Simulation of Vout range

![image](https://github.com/trong420/opamp/assets/90754954/5d2b83c4-1534-4bc0-9fee-85e584110f82)


```bash
source scripts/opt_ctrl.tcl
```
