# Visualizing the Wavefunction and Probability density of a Particle in a 1D Infinite Potential Well

This project demonstrates the visualization of the wavefunction and probability density of a quantum particle confined in a one-dimensional infinite potential well. Using numerical methods, the Schrödinger equation is solved to visualize how the wavefunction evolves for different quantum states within the well. The project allows users to observe key quantum mechanical properties such as energy levels, nodal points, and probability distributions.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [How It Works](#how-it-works)
4. [Concepts](#concepts)
5. [Output](#output)
6. [Conclusion](#conclusion)

## Installation
To run this project on your local machine, ensure that you have the necessary dependencies installed. The following steps outline how to set up the project:

1. Clone this repository:
```
git clone https://github.com/LINSANITY03/Particle-in-Potential-Well
```

2. Create a virtual environment:
```
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install the required dependencies:
```
pip install -r requirements.txt
```

## Usage
After installing the dependencies, go to notebook folder:

```
cd notebook
```
then, open the **main.ipynb** file.

The script will generate visualizations of the wavefunction for various quantum states, including energy levels and probability distributions.

You can modify the parameters in the script from **config.yml** to observe how the wavefunction changes with different particle energies, well sizes, or other variables.

## How It Works
1. **Schrödinger Equation**: The core of this project is the time-independent Schrödinger equation, which governs the wavefunction of a quantum particle. For a particle in a 1D infinite potential well, the equation simplifies to:
$-\frac{\hbar^2}{2m}[ \frac{\partial^2 \psi(x)}{\partial t^2}]=E\psi(x)$
where $\psi(x)$ is the wavefunction, E is the energy, $\hbar$ is the reduced Planck constant, and m is the particle's mass.

2. **Numerical Solution**: Since the Schrödinger equation does not have a simple analytical solution for arbitrary parameters, numerical methods are used to solve for the wavefunction $\psi$ in the potential well.

3. **Visualization**: The resulting wavefunction is plotted as a function of position within the well. Probability distributions are visualized.

## Concepts
This project illustrates the following key concepts from quantum mechanics:

- Quantum States: The wavefunction of a particle in the well can be described by discrete quantum states, each corresponding to a specific energy level.

- Energy Quantization: The energy levels in an infinite potential well are quantized, and the particle can only occupy specific energy states. The energies are given by:
$E_n = \frac{n^2\pi^2\hbar^2}{2mL^2}$
where n is a positive number, and L is the width of the potential well.

- Wavefunction Behavior: The wavefunction exhibits different behaviors for different quantum numbers n. For example:
    - for n = 1, he wavefunction has no nodes and represents the ground state.
    - Higher values of n introduce more nodes and represent excited states.

- Probability Density: The square of the absolute value of the wavefunction $|\psi^2|$ represents the probability density of finding the particle at a given position within the well.

## Output

1. Plot of the wavefunctions and probability density for the first three quantum states.

<p align="center">
  <img src="figures/wave_function.png" alt="Algorithm_game" height="360" width="640">
</p>

<p align="center">
  <img src="figures/probability_density.png" alt="Algorithm_game" height="360" width="640">
</p>

2. Energy levels

The calculated energy levels for the first three quantum states are:

| Quantum State (n) | Energy (Joule) |
| --- | --- |
| 1 | 6.02e-20 |
| 2 | 2.41e-19 |
| 3 | 5.42e-19 |

## Conclusion
This project demonstrates the behavior of a quantum particle in a 1D infinite potential well. The wavefunctions and probability densities exhibit distinct patterns for different quantum states, and the energy levels.

## Collaboration

Feel free to use this codebase for your projects. If you want to talk more about this project or have found bugs, create a pull request or contact me on **pujantamang92@gmail.com**.
