# Evaluation of properties of clustered quantum circuits / Evaluation von Charakteristiken geclusterter Quantenschaltkreise
<!-- markdown-link-check-disable -->
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
<!-- markdown-link-check-enable -->
This project contains the results of the evaluation of clustered quantum circuits.

The research questions are:
- What is the behavior of the circuits as connectivity increases with respect to the metrics?
  - Is there a smooth transition from separable circuits to dense circuits, or is there a tipping point?
  - Is there a difference between different interaction types?
- What arrangement of circuits is advantageous when using clustered circuits for certain metrics?



The result of our research project is:
- The more qubits are entangled with each other through a loop, the better the expressibility values. However, this does not imply that high entanglement presupposes good expressibility values.
- Expressibility of separable circuits < expressibility of loop circuits < expressibility of all-to-all circuits
- Directly comparing the parametrized rotation operations, the insertion of crx and cry achieves significant improvements in expressibility as entanglement is increased.
- When choosing between crx, cry, and crz: crx and cry behave similarly to each other. On the other hand, crz achieves hardly any improvements in expressibility as entanglement hardly changes.
- Increasing the depth can improve expressibility. However, manipulating the width does not show this effect.

## Repository Organization

- `results`: Contains the txt results of our evaluation.
- `implementation`: Contains the automatic clustered circuit generation and the expressibility according to [Sim19] & entangling capability according to [Mey02].
- `docs`: Contains futher explanations for the strategies and decisions.

## Learn More

*	[Hub20] Hubregtsen, T., Pichlmeier, J., Stecher, P., & Bertels, K.. (2020). Evaluation of Parameterized Quantum Circuits: on the relation between classification accuracy, expressibility and entangling capability. https://doi.org/10.48550/arXiv.2003.09887

*	[Mey02] Meyer, David A. & Wallach, Nolan R.. (2002). Global entanglement in multiparticle systems. Journal of Mathematical Physics, 43(9), 4273–4278. 
https://doi.org/10.1063/1.1497700


*	[Sim19] Sim, S., Johnson, Peter D., & Aspuru-Guzik, Alán (2019). Expressibility and Entangling Capability of Parameterized Quantum Circuits for Hybrid Quantum-Classical Algorithms. Advanced Quantum Technologies, 2(12), 1900070. https://doi.org/10.1002/qute.201900070

## License
The self-produced code is available under the Apache-2.0 License.
This project includes parts from third-party libraries. Their use is subject to their license terms. 
The implementation used the following third-party libraries:

* Kim, Saesun & Scholten, Travis L. (2021). Expressibility of Parametrized Quantum Circuits & Classification Accuracy of Quantum Neural Networks. 
The library is licensed under the [MIT License](https://raw.githubusercontent.com/bagmk/Quantum_Machine_Learning_Express/main/LICENSE).
