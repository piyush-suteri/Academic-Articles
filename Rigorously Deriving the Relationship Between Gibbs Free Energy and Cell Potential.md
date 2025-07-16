# From First Principles: Rigorously Deriving the Relationship Between Gibbs Free Energy and Cell Potential, Leading to the Nernst Equation
By Piyush Suteri

Electrochemistry, the study of the interconversion of chemical and electrical energy, is a cornerstone of modern science and technology, powering everything from our mobile devices to large-scale industrial processes. At its heart lies the intricate relationship between the thermodynamic driving force of a chemical reaction, encapsulated by the **Gibbs Free Energy ($\Delta G$)**, and the electrical potential it can generate, known as the **cell potential ($E_{cell}$)**. This article will rigorously derive this fundamental relationship and subsequently, the pivotal **Nernst Equation**, from the bedrock of thermodynamics.

---

## 1. The First Law of Thermodynamics: Energy Conservation

We begin with the First Law of Thermodynamics, which states that the change in internal energy ($dU$) of a system is equal to the heat ($dq$) added to the system minus the work ($dW$) done by the system:

$dU = dq - dW$ (Equation 1)

Here, $dW$ represents the total work done by the system on its surroundings.

---

## 2. The Second Law of Thermodynamics: Entropy and Reversibility

The Second Law introduces the concept of **entropy ($S$)**, a measure of disorder or the dispersal of energy. For a reversible process, the change in entropy ($dS$) is defined as:

$dS = \frac{dq_{rev}}{T}$ or equivalently $dq_{rev} = TdS$ (Equation 2)

where $dq_{rev}$ is the heat transferred during a reversible process and $T$ is the absolute temperature. The concept of "reversible" is critical here: a reversible process occurs infinitesimally slowly, always maintaining equilibrium, thereby yielding the maximum possible useful (non-PV) work.

---

## 3. Defining Enthalpy and Gibbs Free Energy

To manage the complexities of systems involving pressure-volume work, we introduce two useful thermodynamic potentials:

**Enthalpy ($H$)**: Defined as $H = U + PV$. For an infinitesimal change:

$dH = dU + PdV + VdP$ (Equation 3)

Enthalpy is particularly useful for processes occurring at constant pressure.

**Gibbs Free Energy ($G$)**: Defined as $G = H - TS$. For an infinitesimal change:

$dG = dH - TdS - SdT$ (Equation 4)

Gibbs free energy is the most relevant thermodynamic potential for processes occurring at constant temperature and pressure, as it directly relates to the maximum non-PV work a system can perform.

---

## 4. Rigorous Derivation of $\Delta G$ and Non-Expansion Work

Let's substitute Equation 3 into Equation 4:

$dG = (dU + PdV + VdP) - TdS - SdT$ (Equation 5)

Now, we introduce the First Law (Equation 1) into Equation 5. For our purposes, and to connect with the Second Law (which uses $dq_{rev}$), we consider a reversible process. For a reversible process, $dU = dq_{rev} - dW_{total,rev}$.

Let's categorize the total reversible work ($dW_{total,rev}$) done by the system into two components:

* **Expansion (PV) work ($dW_{PV,rev}$)**: This is the work done due to volume change against an external pressure, typically expressed as $PdV$.
* **Non-expansion (non-PV) work ($dW_{non-PV,rev}$)**: This encompasses all other forms of useful work, such as electrical work in an electrochemical cell, mechanical work, etc.

Thus, we can write:

$dW_{total,rev} = dW_{PV,rev} + dW_{non-PV,rev} = PdV + dW_{non-PV,rev}$

Substituting $dU = dq_{rev} - (PdV + dW_{non-PV,rev})$ into Equation 5:

$dG = (dq_{rev} - (PdV + dW_{non-PV,rev}) + PdV + VdP) - TdS - SdT$
$dG = dq_{rev} - PdV - dW_{non-PV,rev} + PdV + VdP - TdS - SdT$

The $PdV$ terms cancel out:

$dG = dq_{rev} - dW_{non-PV,rev} + VdP - TdS - SdT$ (Equation 6)

Now, we apply the Second Law for a reversible process, $dq_{rev} = TdS$ (Equation 2), into Equation 6:

$dG = (TdS) - dW_{non-PV,rev} + VdP - TdS - SdT$

The $TdS$ terms cancel, yielding the fundamental Gibbs Equation:

$dG = -dW_{non-PV,rev} + VdP - SdT$ (Equation 7)

This powerful equation holds for any reversible process. For electrochemical cells, reactions typically occur at **constant temperature ($dT=0$)** and **constant pressure ($dP=0$)**. Under these specific conditions, Equation 7 simplifies significantly:

$dG = -dW_{non-PV,rev}$

Integrating this for a finite change in a reversible process:

$\Delta G = -W_{non-PV,rev}$ (Equation 8)

This is a profound result: the change in Gibbs free energy ($\Delta G$) for a process occurring at constant temperature and pressure is equal to the negative of the maximum reversible non-pressure-volume work that can be done by the system. A negative $\Delta G$ means the system can do positive useful work.

---

## 5. Connecting $\Delta G$ to Electrical Work and Cell Potential ($E_{cell}$)

In an electrochemical cell (e.g., a galvanic cell), the non-PV work is primarily **electrical work**. The infinitesimal electrical work done by the system ($dW_{non-PV,rev}$) is given by the product of the electrical potential difference ($V$) and the infinitesimal charge ($dq$) that traverses this potential difference:

$dW_{non-PV,rev} = Vdq$ (Equation 9)

If the potential difference $V$ approaches the cell's **electromotive force ($E_{cell}$)**, which occurs under open-circuit or equilibrium conditions (when no current or an infinitesimal current is drawn), then $dG = -E_{cell}dq$. Here, $E_{cell}$ represents the electromotive force (EMF) of the cell, which is the maximum potential difference the cell can achieve under reversible conditions.

Substituting Equation 9 into Equation 8 for an infinitesimal change:

$dG = -E_{cell}dq$

For a finite change, if $n$ moles of electrons are transferred during the reaction, the total charge ($q$) transferred is $nF$, where **$F$ is Faraday's constant (96485 C/mol)**, representing the charge of one mole of electrons. Integrating for a process involving $n$ moles of electrons:

$\Delta G = -nFE_{cell}$ (Equation 10)

This is the cornerstone relationship: the change in Gibbs free energy of an electrochemical reaction is directly proportional to the cell's electromotive force ($E_{cell}$), the number of electrons transferred ($n$), and Faraday's constant ($F$). A negative $\Delta G$ (spontaneous reaction) corresponds to a positive $E_{cell}$ (cell generates electricity).

---

## 6. Deriving the Nernst Equation

Equation 10 gives us the relationship between $\Delta G$ and $E_{cell}$ under any conditions (standard or non-standard). To extend this to non-standard conditions, we need another fundamental thermodynamic relation that describes how Gibbs free energy changes with concentrations/pressures:

$\Delta G = \Delta G^\circ + RT\ln Q$ (Equation 11)

Here:

* $\Delta G^\circ$ is the **standard Gibbs free energy change**, which occurs when all reactants and products are in their standard states (1 M concentration for solutes, 1 atm partial pressure for gases, pure solids/liquids, typically at 298.15 K).
* $R$ is the **ideal gas constant (8.314 J/(mol·K))**.
* $T$ is the **absolute temperature in Kelvin**.
* $Q$ is the **reaction quotient**, which expresses the relative amounts of products to reactants at any given time. For a general reaction $aA + bB \rightleftharpoons cC + dD$, $Q = \frac{[C]^c[D]^d}{[A]^a[B]^b}$.

Just as $\Delta G$ is related to $E_{cell}$, the standard Gibbs free energy change ($\Delta G^\circ$) is related to the **standard cell potential ($E_{cell}^\circ$)**, which is the EMF of the cell under standard conditions:

$\Delta G^\circ = -nFE_{cell}^\circ$ (Equation 12)

Now, we substitute Equation 10 and Equation 12 into Equation 11:

$-nFE_{cell} = -nFE_{cell}^\circ + RT\ln Q$

Finally, to arrive at the Nernst Equation, we divide the entire equation by $-nF$:

$E_{cell} = E_{cell}^\circ - \frac{RT}{nF}\ln Q$ (Equation 13)

This is the **Nernst Equation**. It allows us to calculate the cell potential ($E_{cell}$) under any given set of concentrations and temperatures, given the standard cell potential ($E_{cell}^\circ$) and the reaction quotient ($Q$).

---

## 7. Common Form and Significance

While Equation 13 is the general form of the Nernst Equation, it is frequently encountered in a simplified form under specific conditions:

Recall that $\ln x = 2.303\log_{10} x$. Substituting this:

$E_{cell} = E_{cell}^\circ - \frac{2.303RT}{nF}\log_{10} Q$

At 298.15 K, the value of $\frac{2.303RT}{nF}$ is approximately 0.0592 V. Thus, the Nernst Equation becomes:

$E_{cell} = E_{cell}^\circ - \frac{0.0592}{n}\log_{10} Q$ (at 25 °C)

The Nernst equation is indispensable in electrochemistry. It quantifies how concentration gradients drive or oppose electrochemical reactions, enabling the prediction of cell potential in diverse real-world applications, from biological processes to battery design. It stands as a testament to the elegant consistency between macroscopic thermodynamic principles and the microscopic world of electron transfer.
