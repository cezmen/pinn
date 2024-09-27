# PINN Solution for 1D Maxwell's Equations

## 1D cavity model filled with homogeneous media

![Electric Field Equation](https://latex.codecogs.com/png.latex?E_n(x,t)%20=%20E_0%20\sin\left(\frac{n\pi%20x}{L}\right)e^{i%20\omega_n%20t})

and

![Magnetic Field Equation](https://latex.codecogs.com/png.latex?H_n(x,t)%20=%20H_0%20\cos\left(\frac{n\pi%20x}{L}\right)e^{i%20\omega_n%20t})


  <h1>1D Cavity Model with Homogeneous Media</h1>
  <p>
      In the context of the 1D Cavity Model with homogeneous media, <strong>mode numbers</strong> refer to the quantized frequencies of the standing wave solutions for the electric field \(E(x,t)\) and magnetic field \(H(x,t)\) inside the cavity. These modes result from the boundary conditions imposed on the fields, typically at the ends of the cavity (e.g., perfectly conducting walls).
  </p>
  <p>
      The mode numbers \(n\) are related to the <strong>number of half-wavelengths</strong> that fit within the cavity. For a cavity of length \(L\), the mode number determines the possible wave patterns (standing wave configurations) that can form inside the cavity, as described by:
  </p>
  <p>
      \[
      E_n(x, t) = E_0 \sin\left( \frac{n \pi x}{L} \right) e^{i \omega_n t}
      \]
      and
      \[
      H_n(x, t) = H_0 \cos\left( \frac{n \pi x}{L} \right) e^{i \omega_n t}
      \]
  </p>
  <p>
      where:
      <ul>
          <li>\(n\) is the mode number (an integer: \(n = 1, 2, 3, \dots\)),</li>
          <li>\(L\) is the length of the cavity,</li>
          <li>\(\omega_n = \frac{n \pi c}{L}\) is the angular frequency of the mode,</li>
          <li>\(c\) is the speed of light in the medium.</li>
      </ul>
  </p>
  <h2>Meaning of Mode Numbers</h2>
  <p>
      <strong>Mode number \(n = 1\)</strong> corresponds to the fundamental mode, with a single half-wavelength fitting inside the cavity. This is the lowest frequency mode.
  </p>
  <p>
      <strong>Higher mode numbers</strong> (e.g., \(n = 2, 3, \dots\)) correspond to higher harmonics, where additional half-wavelengths fit within the cavity. Each increase in the mode number corresponds to a higher frequency of oscillation.
  </p>
  <p>
      In summary, the mode number controls the spatial variation of the fields, determining how many nodes and antinodes appear along the length of the cavity. Higher mode numbers correspond to more complex standing wave patterns and higher frequencies.
  </p>
