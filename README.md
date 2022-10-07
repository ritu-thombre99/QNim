# QNim

This project is implemented under the guidance of James Weaver as part of QAMP (Qiskit Advocate Mentorship Program) Fall-22. Project description can be found [here](https://github.com/qiskit-advocate/qamp-fall-22/issues/29).

Implementing strategy for quantum computer to play Nim game against human/classical computer.
1. One of the first games in which a human played against the computer is Nim, so it is an interesting and fitting game to implement on a quantum computer. [This](https://en.wikipedia.org/wiki/Nim) Wikipedia article describes the game, strategies and variants.
2. The QC's gameplay strategy is based upon mathematical theory for [Nim](https://en.wikipedia.org/wiki/Nim#Mathematical_theory), played as a misère game. This strategy is implemented using dynamically generated circuit based upon the remaining piles of objects each time it is the QC's turn to play.
3. In case there are winnable moves possible, superposition for these moves is created and the measurement of circuit will decide the qc's move.
4. In case the measurement is nonsense (e.g pick negative objects, pick pile not present on the board, etc) qc automatically loses the game.
