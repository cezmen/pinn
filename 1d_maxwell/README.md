# PINN Solution for 1D Maxwell's Equations

These demos showcase the implementation of Physics-Informed Neural Networks (PINNs) for solving 1D Maxwell's equations in the classical "1D cavity with homogeneous medium" problem. Each demo employs a fully connected neural network with 3 hidden layers, consisting of 24, 12, and 6 neurons, respectively. The input layer has two dimensions (space x and time t), while the output layer predicts both the electric field (Ey) and magnetic field (Hz). Together, these demos illustrate the capability of PINNs to model electromagnetic field dynamics in the cavity across different configurations.

The PINN solution for 1D Maxwell's equations efficiently models electromagnetic fields in the 1D cavity filled with homogeneous media, capturing wave propagation and resonance. This approach enables accurate simulations of field behavior, crucial for applications like waveguides, resonant cavities, and antenna design, without relying on traditional numerical methods.


**<ins>PINN Simulation Results</ins>:**

- :bar_chart: &nbsp; [Mode 1 Example](mode_1/README.md) <br>
- :bar_chart: &nbsp; [Mode 2 Example](mode_2/README.md) <br>
- :bar_chart: &nbsp; [Mode 4 Example](mode_4/README.md) <br>

<br>

**<ins>Source Code for PINN Solution</ins>:**
- :abacus: &nbsp; [Explore Source Code](code/README.md)

<br>

## 1D cavity model filled with homogeneous media (Summary)

In the context of the 1D Cavity Model with homogeneous media, **mode numbers** refer to the quantized frequencies of the standing wave solutions for the electric field $E(x,t)$ and magnetic field $H(x,t)$ inside the cavity. These modes result from the boundary conditions imposed on the fields, typically at the ends of the cavity (e.g., perfectly conducting walls).

The mode numbers $n$ are related to the **number of half-wavelengths** that fit within the cavity. For a cavity of length $L$, the mode number determines the possible wave patterns (standing wave configurations) that can form inside the cavity, as described by the general solution:

$$
E_n(x, t) = E_0 \sin\left( \frac{n \pi x}{L} \right) e^{i \omega_n t}
$$

and

$$
H_n(x, t) = H_0 \cos\left( \frac{n \pi x}{L} \right) e^{i \omega_n t}
$$

where:
- $n$ is the mode number (an integer: $n = 1, 2, 3, \dots$),
- $L$ is the length of the cavity,
- $\omega_n = \frac{n \pi c}{L}$ is the angular frequency of the mode,
- $c$ is the speed of light in the medium.

<br>

## Meaning of Mode Numbers

**Mode number $n = 1$** corresponds to the fundamental mode, with a single half-wavelength fitting inside the cavity. This is the lowest frequency mode.

**Higher mode numbers (e.g., $n = 2, 3, \dots$)** correspond to higher harmonics, where additional half-wavelengths fit within the cavity. Each increase in the mode number corresponds to a higher frequency of oscillation.

In summary, the mode number controls the spatial variation of the fields, determining how many nodes and antinodes appear along the length of the cavity. Higher mode numbers correspond to more complex standing wave patterns and higher frequencies.

<br>

## Common Applications 

The 1D cavity model filled with homogeneous media is a simplified yet powerful framework used to study wave propagation and resonance phenomena. In real-world applications, this model is commonly employed in the design of waveguides, where electromagnetic waves are transmitted through structures such as optical fibers or microwave transmission lines. It also plays a crucial role in understanding resonant cavities, which are used in devices like lasers, microwave ovens, and particle accelerators, to manage and amplify electromagnetic waves. Additionally, this model informs antenna design, aiding in the development of efficient transmission and reception systems by controlling wave behavior and resonance within confined spaces.

<br>

| Application             | Description                                                                                       | Relevance of the 1D Cavity Model                                                          |
|-------------------------|---------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| Waveguides              | Used to guide electromagnetic waves in systems like optical fibers and microwave transmission lines. | The 1D cavity model helps simulate wave propagation and boundary reflections, allowing engineers to optimize signal transmission with minimal distortion or loss. |
| Resonant Cavities        | Utilized in lasers, microwave ovens, and particle accelerators to confine and amplify electromagnetic waves at specific frequencies. | This model accurately predicts the behavior of standing waves and resonant frequencies, enabling efficient energy storage and wave amplification within the cavity. |
| Antenna Design           | Informs the design of antennas by controlling how electromagnetic waves propagate and resonate in confined environments. | The model assists in analyzing the resonant behavior of antennas, ensuring they transmit and receive signals effectively at desired frequencies. |
| Microwave Filters        | Applied in the design of filters to isolate specific frequencies in microwave circuits.            | The 1D cavity model aids in understanding how electromagnetic waves interact with filters, ensuring precise frequency selection and signal purity. |
| Cavity Quantum Electrodynamics (CQED) | Used in quantum technologies to study the interaction between light and matter within a cavity. | By modeling the electromagnetic field in a confined space, the 1D cavity model helps researchers explore light-matter interactions, crucial for advancements in quantum computing and communication. |

<br>

:back: &nbsp; [Return to PINN Applications](../README.md)

