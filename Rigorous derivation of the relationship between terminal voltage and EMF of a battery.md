# A Rigorous Derivation of the Terminal Voltage Equation: $V = \text{emf} - ir$

Let's explore the fundamental principles governing the operation of a battery, starting from an uncharged state and progressing to its behavior in a closed circuit.

## Phase 1: Initial Charge Separation (Battery in Open Circuit)

Consider the material within a battery initially, where charges are uniformly distributed and not separated.

1.  **Development of Battery Force:** Due to some internal mechanism (e.g., chemical reactions in an electrochemical cell), a non-conservative "battery force" ($\vec{F}_b$) develops. This force acts to separate positive and negative charges within the battery material. For a positive charge $q$, $\vec{F}_b$ moves it towards what will become the positive terminal (say, A), and simultaneously an equal and opposite force acts on negative charges, moving them towards the negative terminal (say, B).

2.  **Creation of Electric Field:** As charges begin to accumulate at terminals A and B, they establish an electric field ($\vec{E}$) within the battery material. This electric field, in turn, exerts an electrostatic force ($\vec{F}_e = q\vec{E}$) on the charges within the battery material. Crucially, this force acts in the opposite direction to the battery force, opposing further charge separation.

3.  **Approach to Steady State:** Over time, as more charge accumulates at the terminals, the strength of the opposing electrostatic force ($\vec{F}_e$) increases. Consequently, the net force driving charges towards the terminals ($\vec{F}_b - \vec{F}_e$) decreases.

4.  **Steady State (Open Circuit):** Eventually, a state is reached where the opposing electrostatic force ($\vec{F}_e$) precisely balances the battery force ($\vec{F}_b$). At this point, the net force on charges within the battery material becomes zero, and charge separation ceases. This equilibrium state is referred to as the steady state (for an open-circuit battery). Theoretically, this state will be maintained indefinitely as long as nothing is connected externally to the battery's terminals.

## Defining Electromotive Force (EMF)

The work done by the battery force ($\vec{F}_b$) in moving a positive charge $q$ from the low potential terminal B to the high potential terminal A is denoted as $W_b$. The electromotive force (EMF) of the battery is defined as this work done per unit charge:

$$\text{emf} = \frac{W_b}{q}$$

At the open-circuit steady state, if a charge $q$ were to be hypothetically displaced by an external force from B to A, the work done by the battery force ($W_b$) would be equal to the work done against the electric force ($W_e$). Since $W_e$ is related to the potential difference $V$ across the terminals by $W_e = qV$, it follows that $W_b = qV$. Substituting this into the EMF definition:

$$\text{emf} = \frac{qV}{q} = V$$

Therefore, in the open-circuit steady state, the EMF of the battery equals its terminal voltage.

## Intermediate (Transient) State Analysis

During the initial period when charge separation has begun but the open-circuit steady state has not yet been achieved, there is a net force acting on the charges. The net work done on a charge $q$ by this net force ($W_n$) is the sum of the work done by the battery force ($W_b$) and the work done by the electric force ($W_e$):

$$W_n = W_b + W_e$$

Rearranging this equation, we get $W_b = W_n - W_e$.

Applying the Work-Energy Theorem:
* $W_n$ (net work) equals the change in kinetic energy ($\Delta K$) of the charge: $W_n = \Delta K$.
* $W_e$ (work done by the conservative electric force) equals the negative of the change in electrical potential energy ($\Delta U$) of the system: $W_e = -\Delta U$.

When a positive charge $q$ is moved from a low potential (B) to a high potential (A), the change in potential energy ($\Delta U$) is positive. Therefore, substituting these into the equation for $W_b$:

$$W_b = \Delta K - (-\Delta U) = \Delta K + \Delta U$$

This equation implies that the work done by the battery force on a charge $q$ is distributed: a portion goes into increasing the potential energy of the system ($\Delta U$), and the remaining portion goes into increasing the kinetic energy of the charge ($\Delta K$).

It's important to note that if the kinetic energy of the charges increases, this leads to more frequent collisions within the battery material, which in turn increases the temperature of the system. As the system approaches the open-circuit steady state, the net force decreases, and consequently, $\Delta K$ also decreases, approaching zero.

## Phase 2: Battery Connected to an External Closed Circuit

Now, let's consider what happens when the battery is connected to an external closed circuit, allowing current to flow.

1.  **Charge Extraction and Voltage Drop:** As the external circuit begins to draw charges from the battery (creating an external current), the charge accumulation at the terminals starts to decrease. This leads to a reduction in the electric potential difference across the battery's terminals.

2.  **Weakening $\vec{F}_e$ and Dominant $\vec{F}_b$:** Due to the drop in terminal voltage, the opposing electrostatic force ($\vec{F}_e$) within the battery weakens, while the battery force ($\vec{F}_b$) remains essentially constant (as it's driven by the internal mechanism).

3.  **Counteracting Depletion (Transient State):** As the terminal voltage tends to drop further, the net force ($\vec{F}_b - \vec{F}_e$) on charges within the battery material becomes significant. This net force acts to counteract the charge depletion at the terminals by driving more charges towards them. Initially, when charge is extracted, the battery's internal mechanism takes a very short time to respond and supply charges at the necessary rate. During this brief period, some charge is already drawn from the terminals, causing an initial dip in the terminal voltage. Let us say total charge accumulated at the positive terminal was $Q$ in the open-circuit steady state, and $q'$ charge is drawn when the circuit is closed. This very short period is known as the transient state.

4.  **New Steady State (Closed Circuit):** Soon after the transient state, as the battery force becomes dominant, the battery's mechanism starts supplying charges to the terminals at a rate that matches the rate at which they are being extracted. Consequently, the current flowing inside the battery becomes equal to the current flowing outside in the external circuit. Because the rate of charge supplied matches the rate of charge extracted, the net charge accumulated at the battery terminals remains constant over time. This implies that the charge separation within the battery also remains constant, and thus the terminal voltage stabilizes at a constant value.

    However, the charge lost from the positive terminal ($q'$) during the transient state is not recovered, and the final charge accumulation at the positive terminal remains $Q - q'$. Due to the extent of charge distribution being reduced after the transient state, the terminal voltage becomes less than the EMF of the battery. This is the new steady state for the battery operating in a closed circuit. In this state, since the terminal voltage is less than the EMF, $\vec{F}_e$ is less than $\vec{F}_b$, meaning the battery force ($\vec{F}_b$) is continuously dominant. This continuous dominance of $\vec{F}_b$ allows the battery to constantly supply charges to its terminals, thereby maintaining a stable potential difference across them. This continuous maintenance of a constant potential difference is the defining purpose of a battery in a circuit.

## Energy Analysis in the Closed-Circuit Steady State

Let's re-examine the energy relation $W_b = \Delta K + \Delta U$ in this closed-circuit steady state.

Since the battery force ($\vec{F}_b$) is always dominant and there's a continuous current, the net force is never zero, which means $\Delta K$ (the change in kinetic energy of charges within the battery) is never zero.

A battery is a complex system involving the movement of many charge carriers (ions, electrons). These charges do not simply move in a perfectly directed path; they constantly collide with other particles within the battery material. This continuous process of collisions converts the ordered kinetic energy associated with the current flow into disordered kinetic energy, which is perceived macroscopically as thermal energy. Thus, the portion of the battery's work that goes into increasing $\Delta K$ is effectively dissipated as heat, increasing the temperature of the battery. The remaining portion ($\Delta U$, which is now constant for the steady state) goes into maintaining the potential difference across the terminals, supplying energy to the external circuit.

## Connecting to the Classical Equation: $V = \text{emf} - ir$

To connect this first-principles understanding to the classical circuit equation, we divide the energy relation $W_b = \Delta K + \Delta U$ by the charge $q$ and rearrange the terms:

$$\frac{\Delta U}{q} = \frac{W_b}{q} - \frac{\Delta K}{q}$$

Let's clarify the terms:

* $\frac{W_b}{q}$ is, by definition, the EMF of the battery.
* $\frac{\Delta U}{q}$ represents the electrical potential energy gained per unit charge as it traverses the battery, which corresponds to the terminal voltage ($V$) across the battery.

Substituting these into the equation, we get:

$$V = \text{emf} - \frac{\Delta K}{q}$$

We can write $\Delta K = qir$. You might be wondering how we introduced this expression out of nothing! Observe that $qi$ is constant, so $r$ has to take such a value that makes the equality hold. The term $r$ is nothing more than a convenient symbol, but it makes the expression look like Joule’s law of heating ($qir = (it)(ir) = i^2rt$) and, more importantly, helps us to write the equation in terms of current ($i$), which we are usually concerned with. The quantity $r$ is named the internal resistance of the battery. Classically, when current flows through the battery, it is said to have an internal resistance ($r$), which causes the dissipation of energy as heat.

We can equate the $\frac{\Delta K}{q}$ term with $ir$:

$$V = \text{emf} - ir$$

It is important to understand the nature of the heat energy generated here. In the context of an external resistor, Joule heating ($i^2R$) occurs because electrical potential energy supplied by the source is converted into thermal energy. However, for the heat generated within the battery due to its internal resistance, the energy source is the battery's chemical energy. A portion of the work done by the battery’s force, instead of being converted into electrical potential energy, is converted into thermal energy within the battery itself due to the internal resistive processes (the collisions described by $\Delta K$). Therefore, while both phenomena result in $i^2R$ (or $i^2r$) heating, the fundamental energy conversion pathways differ.

Finally, a clarification regarding $V$ in $V = \text{emf} - ir$: This $V$ refers to the terminal potential difference of the battery (potential at the positive terminal minus the potential at the negative terminal). This is distinct from the concept of "potential drop" used in Ohm's law across a passive element, where "potential drop" typically refers to the decrease in potential in the direction of current flow. The internal mechanism of a battery is generally a chemical reaction. Thus, the battery converts chemical energy into useful electrical energy and unnecessary heat energy by doing work on charges in its material. Such a battery is known as an electrochemical cell.
