# current-mirror
A current mirror circuit that transfers a reference current from one branch to another, resulting in a stable and consistent output current.  It is commonly made up of two identical transistors (BJTs or MOSFETs), with their bases/gates coupled together to ensure similar voltage conditions.  The first transistor (M1) is wired with a resistor to establish a reference current, which governs the output current of the second transistor (M2).  Since both transistors have the same  gate-source voltage, M2 replicates the current flowing through M1,  This circuit is commonly used in analog IC design, biasing circuits, and active loads to provide a constant current source that is unaffected by voltage variations.
## Given:-
power=1mw, Vdd=1.8v, Av>10v/v
### Aim :-
Design for current mirror ratios of 1:1 or 1:2, then do a DC analysis, Change the current mirror ratio in different scenarios and perform DC, AC, and transient analyses and design a differential amplifier using a current mirror circuit and analyze DC, AC, and transients.
## Circuit Diagram :-
![Screenshot 2025-03-24 145621](https://github.com/user-attachments/assets/ed7e5056-1283-4c3d-9a91-7a1371cc51cb)
## case 1
### DC analysis
![Screenshot 2025-03-24 151615](https://github.com/user-attachments/assets/6ade5ae3-2338-4f18-b06b-72283aab95fe) ![Screenshot 2025-03-24 151720](https://github.com/user-attachments/assets/9af4a75f-f9b1-4c13-a10f-410d6daf464c)

| Parameters       | M1   | M2   | M3   |
|-----------------|------|------|------|
| **Model**       | PMOS | PMOS | NMOS |
| **Length**      | 180nm | 180nm | 180nm |
| **Width**       | 20um  | 20um  | 20um  |
| **Expected Current** | 0.277mA | 0.277mA | 0.277mA |
## AC Analysis
![Screenshot 2025-03-30 121227](https://github.com/user-attachments/assets/11dcc42f-4519-429a-a01b-645a541a714c)
## Transient Analysis
![Screenshot 2025-03-30 121237](https://github.com/user-attachments/assets/ca3bdd78-c161-49a3-8c2a-1b56ab3b2115)
## Case 2
![Screenshot 2025-03-24 151110](https://github.com/user-attachments/assets/16424c4f-9477-492f-9f9c-f00742c38fd4)  ![Screenshot 2025-03-24 151830](https://github.com/user-attachments/assets/cd4f6d14-c692-4112-b012-6c5ca5772fd0)


![Screenshot 2025-03-24 151819](https://github.com/user-attachments/assets/61dac50b-9a88-48d9-b8be-b8accdfddd8e)
| Parameters       | M1   | M2   | M3   |
|-----------------|------|------|------|
| **Model**       | PMOS | PMOS | NMOS |
| **Length**      | 400nm | 400nm | 400nm |
| **Width**       | 40um  | 40um  | 40um  |
| **Expected Current** | 0.277mA | 0.277mA | 0.277mA |
## AC Analysis
![Screenshot 2025-03-30 121657](https://github.com/user-attachments/assets/0a84c64d-8f5d-4b7a-aae2-d6b6fcf7c54d)
## Transient Analysis
![Screenshot 2025-03-30 121710](https://github.com/user-attachments/assets/93888de6-f45a-4cf4-9bb1-26f52f375b12)
## Current mirror with differential amplifier 
A current mirror circuit combined with a differential amplifier is a typical architecture in analog circuits, particularly in operational amplifiers (op-amps) and analog integrated circuits.  The **current mirror** serves as a **active load** for the differential amplifier, maintaining a constant current through the differential pair while increasing gain and common-mode rejection.  In this configuration, the **differential pair** is made up of two transistors (BJTs or MOSFETs) that receive two input signals each.  The **current mirror** replaces the typical resistor load, giving a constant current source and guaranteeing that the differential pair runs smoothly.  This improves the amplifier's **gain, linearity, and performance**, making it suitable for applications that require high precision, such as sensor interfaces and analog computation.
## Circuit diagram 
![Screenshot 2025-03-30 130823](https://github.com/user-attachments/assets/f6756fd8-4072-4d4b-8519-bb47cdd153d3)
### DC analysis
![image](https://github.com/user-attachments/assets/de262ddb-afc9-42c8-b20c-0a39c9a80d2c)
## AC analysis
![image](https://github.com/user-attachments/assets/cccc131b-8401-4650-945a-f5e382bf49a1)
## Transient analysis
![Screenshot 2025-03-30 130804](https://github.com/user-attachments/assets/874065b9-f054-4ca0-a3d1-65b340b85a93)
## conclusion
Current mirrors improve circuit stability and efficiency, making them essential for integrated circuits, op-amps, and analog signal processing.
A current mirror circuit is a fundamental building component in analog design, providing a stable and precise current source that is unaffected by voltage fluctuations.  It guarantees accurate current replication, which is required for biasing, active loads, and differential amplifier circuits.  While an ideal current mirror ensures perfect current matching, practical restrictions like as transistor mismatches, temperature changes, and output resistance cause minor variances.
## Inference
The current mirror circuit successfully matches a reference current in another branch, resulting in a stable and exact current source.  
This experiment indicates that the reflected current is substantially equivalent to the reference current, demonstrating its usefulness for biasing, active loads, and signal amplification.  
practical issues such as transistor mismatches, temperature changes, and finite output resistance create minor deviations from the ideal performance.
