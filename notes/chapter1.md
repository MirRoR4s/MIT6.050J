# Chapter 1

### 1.5.1 An Advantage of Qubits

There are things that can be done in a quantum context but not classically. Some are advantageous. Here is one example:

Consider again Alice trying to send information to Bob using polarized photons. She prepares photons that have either horizontal or vertical polarization, and tells that to Bob, during the setup phase. Now let us suppose that a saboteur（破坏者）Sam wants to spoil（破坏） this communication by processing the photons at some point in the path between Alice and Bob. He uses a machine that simple measures the polarization at an angle he selects. If he selects $45^{\circ}$, every photon ends up with a polarization at the angle or perpendicular to it, regardless of its original polarization. Then Bob, making a vertical measurement, will measure 0 half the time and 1 half the time, regardless of what Alice sent.

Alice learns about Sam's scheme and wants to reestablish reliable communication with Bob. What can she do?

She tells Bob (using a path that Sam does not overhear) she will send photons at $45\circ$ and $135\circ$, so he should measure at one of those angles. Sam's machine then does not alter the pohtons. Of course if Sam discovers what Alice is doing, he can rotate his machine back to vertical. Or there are other measures and counter-measures that could be put into action.

This scenario（场景）relies on the quantum nature of the photons, and the fact that single photons cannot be measured by Sam except along particular angles of polarization. Thus Alice's technique for thwarting（阻挠） Sam is not possible with classical bits.

---

## 1.6 The Classical Bit

Because quantum measurement generally alters the object being measured, a quantum bit cannot be measured a second time. On the other hand, if a bit is represented by many objects with the same properties, then after a measurement enough objects can be left unchanged so that the same bit can be measured again.

In today's electronic systems, a bit of information is carried by many objects, all prepared in the same way (or at least that is a convenient way to look at it). Thus in a semiconductor-半导体 memory a single bit is represented by the presence or absence of perhaps 60,000 electrons-电子 (stored on a 10 fF capacitor-电容器 charged to 1V). Similarly, a large number of photons are used in radio communication-无线电通信.

Because many objects are involved, measurements on them are not restricted to a simple yes or no, but instead can range over a continuum of values. Thus the voltage on a semiconductor logic element might be anywhere in a range from, say, 0V to 1V. The voltage might be interpreted to allow a margin of error-误差范围, so that voltages between 0V and 0.2V would represent logical 0, and voltages between 0.8V and 1V a logical 1. The circuitry-电路系统 would not guarantee to interpret voltages between 0.2V and 0.8V properly. If the noise in a circuit is always smaller than 0.2V, and the output of every circuit gate is either 0V or 1V, then the voltages can always be interpreted as bits without error.

Circuits of this sort display what is known as "restoring logic"-恢复逻辑 since small deviations-偏差 in voltage from the ideal values of 0V and 1V are eliminated as the information is precessed. The robustness of modern computers depends on the use of restoring logic.

A classical bit is an abstraction in which the bit can be measured without perturbing-扰乱 it. As a result copies of a classical bit can be made. This model works well for circuits using restoring logic.

Because all physical systems ultimately obey quantum mechanics, the classical bit is always an approximation to reality. However, even with the most modern, smallest devices available, it is an excellent one.  An interesting question is whether the classical bit approximation will continue to be useful as advances in semiconductor technology allow the size of components to be reduced. Ultimately, as we try to represnet or control bits with a small number of atoms-原子 or photons, the limiting role of quantum mechanics will become important. It is diffcult to predice exactly when this will happen, but some people believe it will be before the year 2015.

---

## 1.7 Summary

There are several models of a bit, useful in different contexts. These models are not all the same. In the rest of these notes, the Boolean bit will be use most often, but sometimes the quantum bit will be needed.
