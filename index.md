## Quantum Computing


### What is Quantum Computing?
Quantum computing is the use of quantum phenomena such as superposition and entanglement to perform computation. Computers that perform quantum computations are known as quantum computers. Quantum computers are believed to be able to solve certain computational problems, such as integer factorization (which underlies RSA encryption), substantially faster than classical computers. The study of quantum computing is a subfield of quantum information science.


### Quantum bits

Quantum bits (or “qubits”) are made of subatomic particles, namely individual photons or electrons. Because these subatomic particles conform more to the rules of quantum mechanics than classical mechanics, they exhibit the bizarre properties of quantum particles. The most salient of these properties for computer scientists is superposition. This is the idea that a particle can exist in multiple states simultaneously, at least until that state is measured and collapses into a single state. By harnessing this superposition property, computer scientists can make qubits encode a 1 and a 0 at the same time.

### Quantum Entanglement

The other quantum mechanical quirk that makes quantum computers tick is entanglement, a linking of two quantum particles or, in this case, two qubits. When the two particles are entangled, the change in state of one particle will alter the state of its partner in a predictable way, which comes in handy when it comes time to get a quantum computer to calculate the answer to the problem you feed it.

### Potential Applications

#### Cryptography
Integer factorization, which underpins the security of public key cryptographic systems, is believed to be computationally infeasible with an ordinary computer for large integers if they are the product of few prime numbers (e.g., products of two 300-digit primes). By comparison, a quantum computer could efficiently solve this problem using Shor's algorithm to find its factors. This ability would allow a quantum computer to break many of the cryptographic systems in use today, in the sense that there would be a polynomial time (in the number of digits of the integer) algorithm for solving the problem. In particular, most of the popular public key ciphers are based on the difficulty of factoring integers or the discrete logarithm problem, both of which can be solved by Shor's algorithm. In particular, the RSA, Diffie–Hellman, and elliptic curve Diffie–Hellman algorithms could be broken. These are used to protect secure Web pages, encrypted email, and many other types of data. Breaking these would have significant ramifications for electronic privacy and security.

However, other cryptographic algorithms do not appear to be broken by those algorithms. Some public-key algorithms are based on problems other than the integer factorization and discrete logarithm problems to which Shor's algorithm applies, like the McEliece cryptosystem based on a problem in coding theory. Lattice-based cryptosystems are also not known to be broken by quantum computers, and finding a polynomial time algorithm for solving the dihedral hidden subgroup problem, which would break many lattice based cryptosystems, is a well-studied open problem. It has been proven that applying Grover's algorithm to break a symmetric (secret key) algorithm by brute force requires time equal to roughly 2n/2 invocations of the underlying cryptographic algorithm, compared with roughly 2n in the classical case, meaning that symmetric key lengths are effectively halved: AES-256 would have the same security against an attack using Grover's algorithm that AES-128 has against classical brute-force search (see Key size).

Quantum cryptography could potentially fulfill some of the functions of public key cryptography. Quantum-based cryptographic systems could, therefore, be more secure than traditional systems against quantum hacking.

#### Quantum search
Besides factorization and discrete logarithms, quantum algorithms offering a more than polynomial speedup over the best known classical algorithm have been found for several problems, including the simulation of quantum physical processes from chemistry and solid state physics, the approximation of Jones polynomials, and solving Pell's equation. No mathematical proof has been found that shows that an equally fast classical algorithm cannot be discovered, although this is considered unlikely. However, quantum computers offer polynomial speedup for some problems. The most well-known example of this is quantum database search, which can be solved by Grover's algorithm using quadratically fewer queries to the database than that are required by classical algorithms. In this case, the advantage is not only provable but also optimal, it has been shown that Grover's algorithm gives the maximal possible probability of finding the desired element for any number of oracle lookups. Several other examples of provable quantum speedups for query problems have subsequently been discovered, such as for finding collisions in two-to-one functions and evaluating NAND trees.

There is no searchable structure in the collection of possible answers,
The number of possible answers to check is the same as the number of inputs to the algorithm, and
There exists a boolean function which evaluates each input and determines whether it is the correct answer
For problems with all these properties, the running time of Grover's algorithm on a quantum computer will scale as the square root of the number of inputs (or elements in the database), as opposed to the linear scaling of classical algorithms. A general class of problems to which Grover's algorithm can be applied[22] is Boolean satisfiability problem. In this instance, the database through which the algorithm is iterating is that of all possible answers. An example (and possible) application of this is a password cracker that attempts to guess the password or secret key for an encrypted file or system. Symmetric ciphers such as Triple DES and AES are particularly vulnerable to this kind of attack. This application of quantum computing is a major interest of government agencies.

#### Quantum simulation
Since chemistry and nanotechnology rely on understanding quantum systems, and such systems are impossible to simulate in an efficient manner classically, many believe quantum simulation will be one of the most important applications of quantum computing. Quantum simulation could also be used to simulate the behavior of atoms and particles at unusual conditions such as the reactions inside a collider.

#### Quantum annealing and adiabatic optimization
Quantum annealing or Adiabatic quantum computation relies on the adiabatic theorem to undertake calculations. A system is placed in the ground state for a simple Hamiltonian, which is slowly evolved to a more complicated Hamiltonian whose ground state represents the solution to the problem in question. The adiabatic theorem states that if the evolution is slow enough the system will stay in its ground state at all times through the process.

#### Solving linear equations
The Quantum algorithm for linear systems of equations, or "HHL Algorithm", named after its discoverers Harrow, Hassidim, and Lloyd, is expected to provide speedup over classical counterparts.

#### Quantum supremacy
John Preskill has introduced the term quantum supremacy to refer to the hypothetical speedup advantage that a quantum computer would have over a classical computer in a certain field. Google announced in 2017 that it expected to achieve quantum supremacy by the end of the year though that did not happen. IBM said in 2018 that the best classical computers will be beaten on some practical task within about five years and views the quantum supremacy test only as a potential future benchmark. Although skeptics like Gil Kalai doubt that quantum supremacy will ever be achieved, in October 2019, a Sycamore processor created in conjunction with Google AI Quantum was reported to have achieved quantum supremacy, with calculations more than 3,000,000 times as fast as those of Summit, generally considered the world's fastest computer. Bill Unruh doubted the practicality of quantum computers in a paper published back in 1994. Paul Davies argued that a 400-qubit computer would even come into conflict with the cosmological information bound implied by the holographic principle.

### Research
