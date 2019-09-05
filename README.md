# AQUADUCT
We advance the Coupled Cluster method’s foray into the time-dependent realm, 
byplementing a robust solver based on the orbital-adaptive time-dependent
Coupled Cluster (OATDCC) method. This involves implementing both a simplified static
orbital time-dependent coupled cluster solver with single and double excitations
(TDCCSD) and an orbital-adaptive scheme with double excitations (OATDCCD). To
supplement the time-dependent methods we implement several ground state solvers based
on the Lagrangian Coupled Cluster formulation, with single and double excitations, as
well as a non-orthogonal orbital-optimised Coupled Cluster (NOCC) solver.

We construct several quantum dot basis sets with different potential functions in
one- and two dimensions, including interactions with magnetic fields. What is more, we
also implemet an interface with popular quantum chemistry software modules PySCF and
Psi4 for extraction of additional basis sets for atoms and molecules. The quantum
systems are allowed to vary with time by addition of a time-dependent addition to the
Hamiltonian, with which we simulate a laser field in the dipole approximation.

As a validation we reproduce results from the scientific literature, both for atoms,
molecules and quantum dots. We show that our methods leads to convergence in the
ever-increasing basis set size limit, for simple quantum dot systems. For the same
quantum dot system, we show the sensitivity of the system to the frequency of a driving
oscillating field. Frequencies closer to the resonant frequency leads to exctiations
and increased energy. We are able to simulate systems that are fairly large - quantum
dots in one- and two dimensions with up to twelve electrons. For systems that meander
far from the reference state, we show that the orbital-adaptive method has far superior
stability, compared with the method with static orbitals.

For all quantum dot system we find strong comformity with the harmonic potential
theorem, yet we see slight many-body effect for a two-dimensional double dot system.
The two-dimensional quantum dots influenced by a homogoenous, static magnetic field in
the form of an angular momentum operator, result in a split in the dipole spectrum of
the system. This is also in accordance with the harmonic potential theorem. The
difference between the two frequencies in the new spectrum is the same as the Larmor
frequency of the magnetic field, within acceptable tolerance levels.
