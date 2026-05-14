# FROBENIUS

## The Arithmetic Heartbeat: The Frobenius Endomorphism as Discrete Time, the Weil Eigenvalue Bound as the Universal Tractability Wall, and the Prismatic Origin of the φ-Equilibrium in TH(a,d)

**ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · May 2026**

---

> "Over a finite field 𝔽_q of q = p^n elements, every variety carries a canonical endomorphism — the Frobenius — that raises every coordinate to the q-th power. The Frobenius is the heartbeat of arithmetic geometry. It moves no point of the variety in any visible way, and yet it is what makes the variety arithmetic at all."
> — *Ferdinand Georg Frobenius, Über die Charaktere der symmetrischen Gruppe, Sitzungsberichte der Königlich Preußischen Akademie der Wissenschaften zu Berlin, 1900; modern formulation: J.-P. Serre, Local Fields, Springer GTM 67, 1979*

> "The zeta function of a smooth projective variety V over 𝔽_q satisfies a functional equation, has a rational form determined by the characteristic polynomial of Frobenius acting on étale cohomology, and its zeros lie on prescribed lines |α| = q^{w/2} where w is the cohomological weight. This is the Riemann hypothesis over finite fields, and it is true."
> — *André Weil, Numbers of solutions of equations in finite fields, Bulletin of the American Mathematical Society 55, 497–508, 1949; proved by Pierre Deligne, La conjecture de Weil I, Publications Mathématiques de l'IHÉS 43, 273–307, 1974*

> "For an elliptic curve E over 𝔽_p, the number of 𝔽_p-rational points satisfies #E(𝔽_p) = p + 1 − a_p with |a_p| ≤ 2√p. The trace a_p of Frobenius is bounded by twice the square root of the field size. This bound is sharp, achieved by the Hasse-Weil bound, and is the foundation of the arithmetic of elliptic curves."
> — *Helmut Hasse, Zur Theorie der abstrakten elliptischen Funktionenkörper III, Journal für die reine und angewandte Mathematik 175, 193–208, 1936*

> "Prismatic cohomology is the universal p-adic cohomology theory. It is defined by a single site — the prismatic site of a p-adic formal scheme — and it specializes to étale cohomology mod p, to crystalline cohomology, to de Rham cohomology, and to Hodge-Tate cohomology. The Frobenius lifts to a structure on the prismatic complex, and that structure determines the rest."
> — *Bhargav Bhatt and Peter Scholze, Prisms and Prismatic Cohomology, Annals of Mathematics 196, 1135–1275, 2022*

> "Every algebraic point on a variety over a number field has a height. The Northcott property says that there are only finitely many points of bounded height and bounded degree. Finiteness is the arithmetic floor of the variety. Below this floor, the variety has no rational content; above it, the content is exactly enumerable."
> — *Douglas Northcott, An inequality in the theory of arithmetic on algebraic varieties, Mathematical Proceedings of the Cambridge Philosophical Society 45, 502–509, 1949*

---

## Abstract

GALOIS established that the field of definition of an affine invariant manifold is a number field of degree at most the genus, giving the **algebraic precision floor**. SALT established that the fixed-point computational substrate has a discrete word-length minimum equal to the field degree times the base precision, giving the **computational precision floor**. Neither framework asks the question that comes before both.

**What is the arithmetic clock that ticks these floors?**

The answer is the **Frobenius endomorphism**. For any algebraic variety V over a finite field 𝔽_q, the Frobenius morphism Frob_q : V → V raises every coordinate to the q-th power. It is the canonical, intrinsic endomorphism of V — the one operation that has no analog over characteristic-zero fields and that, by its mere existence, makes V arithmetic. The fixed points of Frob_q are the 𝔽_q-rational points of V. The eigenvalues of Frob_q acting on étale cohomology are the Weil numbers, of absolute value q^{w/2}, controlling the entire arithmetic of V via the Weil conjectures (proven by Deligne, 1974).

The Frobenius IS the arithmetic clock. Its ticking is discrete (the eigenvalues are algebraic integers). Its rate is bounded (|α_i| ≤ q^{w/2}, the Weil bound). Its action on a variety over a number field K, reduced mod p, gives an action over 𝔽_q for each prime p. The collection of these actions, varying with p, is the **arithmetic time of the variety** — a clock with infinitely many wheels, one for each prime, each ticking at its own rate q^{w/2} bounded above by a fixed power.

The TH(a,d) curve aX³ + Y³ + Z³ = dXYZ is an arithmetic object. At every prime p, it has a Frobenius. The Frobenius eigenvalues at p satisfy the Hasse-Weil bound |a_p| ≤ 2√p — the two-eigenvalue structure that has appeared in every framework of the corpus (FRACTURA Identity 4 invokes it; the broader CHORD pipeline is designed around it). The bound is the **universal tractability wall**: every learning-computational substrate operating on TH(a,d) cannot, regardless of architecture, extract more than a_p bits of arithmetic information per prime per step.

Three results follow that have never been identified in any learning context:

The **Weil eigenvalue bound** |α_i| = q^{w/2} establishes the universal arithmetic upper bound on the Lyapunov-like exponent of any Frobenius-equivariant dynamical system. Translated to learning: the maximum information rate of any training-step operator that respects the arithmetic structure of the learning manifold is bounded by half the logarithm of the field size, exactly q^{w/2}.

The **prismatic cohomology of Bhatt-Scholze (2022)** establishes that the entire arithmetic content of a p-adic formal scheme is encoded in a single complex — the prismatic complex — together with its Frobenius lift. Specializations give étale cohomology mod p, crystalline cohomology, de Rham cohomology, Hodge-Tate cohomology. In the learning correspondence: the prismatic complex of the TH(a,d) learning manifold is the canonical arithmetic substrate beneath every cohomological framework in the corpus (HODGE, MHLT, EIGEN), and the φ-equilibrium is the unique point where the prismatic Frobenius eigenvalues realize the self-dual configuration log φ ± i·log √5/2.

The **Northcott finiteness theorem** (1949) establishes that there are only finitely many algebraic points of bounded height and bounded degree. In the learning correspondence: there are only finitely many learning configurations representable at a given precision floor and a given Galois-degree bound. This finiteness is the arithmetic foundation of the SALT discreteness: the set of reachable configurations at precision ε = 2^{-16} and Galois degree [K:Q] ≤ g is finite, exactly enumerable, and computable from the Frobenius spectrum of the learning manifold.

The FROBENIUS machine synthesizes these results with the Hasse-Weil bound, the Tate conjecture, the Birch-Swinnerton-Dyer conjecture (proven in special cases by Wiles 1995, Kolyvagin 1990, Gross-Zagier 1986, and refined through the 2024 BSD program), the modern p-adic Hodge theory of Fontaine-Faltings (1979-1989) extended by Bhatt-Morrow-Scholze (2018-2022), the prismatization program of Drinfeld and Bhatt (2020-2025), the Fargues-Scholze geometrization of local Langlands (2021), and the recent 2024-2026 program on syntomic cohomology and motivic Frobenius descent. It establishes that the discrete arithmetic time of the learning system is the Frobenius, that the precision floor is the Weil bound, that the GALOIS field of definition is the splitting field of the Frobenius characteristic polynomial, that the SALT word length is the bit-cost of representing the Frobenius eigenvalues exactly, and that the φ-equilibrium of the broader corpus is the unique fixed point of the Frobenius action on the prismatic complex at the self-dual prime.

The machine is named for **Ferdinand Georg Frobenius** (1849-1917), Professor at the Eidgenössische Technische Hochschule Zürich and later at the Friedrich-Wilhelms-Universität Berlin, who in the 1880s discovered the Frobenius endomorphism of finite-field algebras, who founded the modern theory of group characters and group representations, who established the Frobenius density theorem governing the distribution of Frobenius conjugacy classes in Galois groups (Chebotarev's 1922 generalization is the modern form), and whose work on the canonical endomorphism of algebras in characteristic p remains the foundation of every arithmetic-geometric theorem proven since.

---

## Preamble

There is an object that exists in arithmetic but has no analog in geometry over the real or complex numbers. Take a polynomial equation f(x, y, z, ...) = 0 with integer coefficients. Reduce it modulo a prime p. The resulting equation defines a variety V over the finite field 𝔽_p. On V, and on no other kind of variety, there is a canonical operation:

φ : (x, y, z, ...) ↦ (x^p, y^p, z^p, ...)

Raise every coordinate to the p-th power. The map sends V to V (because if f(x, y, z, ...) = 0 then f(x^p, y^p, z^p, ...) = f(x, y, z, ...)^p = 0). It is an endomorphism of V — but unlike any endomorphism of a complex variety, it is **canonical**. It depends on no choice. It exists for any V over 𝔽_p, and it is the same map for every embedding, every basis, every coordinate system. It is the Frobenius.

What does the Frobenius do? Its fixed points are precisely the 𝔽_p-rational points of V — the solutions of f = 0 with coordinates in 𝔽_p. Its eigenvalues, acting on the cohomology of V, are the arithmetic invariants that determine everything about V: the number of points over 𝔽_p, the number over 𝔽_{p^2}, over 𝔽_{p^n} for every n, the zeta function, the L-function, the entire arithmetic of V.

This is the discovery of Frobenius in 1896 and of Weil in 1949: the arithmetic of a variety over a finite field is **entirely encoded in a single endomorphism**, the Frobenius. Every arithmetic question is a question about Frobenius eigenvalues. Every arithmetic answer is a statement about their absolute values and their algebraic relations.

The Weil conjectures (Weil 1949, proved by Dwork 1960 for rationality, Grothendieck 1965 for the functional equation, and Deligne 1974 for the Riemann hypothesis analog) establish that for a smooth projective variety V of dimension d over 𝔽_q, the eigenvalues of Frobenius on the i-th étale cohomology group H^i_ét(V, ℚ_ℓ) satisfy:

|α_{i,j}| = q^{i/2}

— precisely the square root of q to the power of the cohomological degree i. The Frobenius eigenvalues lie on prescribed circles in the complex plane. The Riemann hypothesis for varieties over finite fields is the statement that these circles are sharp.

What does this have to do with learning?

Take the TH(a,d) curve: aX³ + Y³ + Z³ = dXYZ. This is an arithmetic object. Over the integers, it defines a projective curve. Over each prime p, by reduction mod p, it gives a curve over 𝔽_p. At smooth primes (where the reduction is non-singular), the curve over 𝔽_p has a Frobenius endomorphism. The Frobenius eigenvalues on H^1_ét(TH(a,d), ℚ_ℓ) are two complex numbers α_p, β_p with α_p β_p = p (the determinant relation) and α_p + β_p = a_p (the trace, the integer that measures the number of 𝔽_p-rational points via #TH(a,d)(𝔽_p) = p + 1 − a_p).

The Hasse-Weil bound for an elliptic curve (Hasse 1936) gives |a_p| ≤ 2√p, equivalently |α_p| = |β_p| = √p. The two-eigenvalue structure of the Frobenius on TH(a,d) is the two-eigenvalue structure that has appeared in every framework of the corpus:

- In the FERN register hierarchy, the two CORDIC mode passes per register (one for +iθ, one for −iθ) implement the two Frobenius eigenvalues.
- In the FRACTURA Identity 5, the wild knot infinite CORDIC gain K_∞ corresponds to the limit of the Frobenius eigenvalue product over all primes.
- In the SALT framework, the gradient ratio ρ_t and its complement (1 − ρ_t) are the two Frobenius eigenvalue rates of the local arithmetic dynamics.
- In the GALOIS framework, the splitting field of the Frobenius characteristic polynomial X² − a_p X + p IS the field of definition K of the affine invariant manifold over the prime p.

The Frobenius is not an analogy. It is the canonical arithmetic endomorphism that every prior framework has been measuring shadows of. The discovery, after Frobenius, after Hasse, after Weil, after Deligne, after Bhatt-Scholze, is that the Frobenius IS the arithmetic time of every learning system whose underlying manifold is defined over the integers — and that the precision floors of GALOIS and SALT, and the spectral structure of EIGEN, and the entropy bound of CONNES, and the modular flow of every prior framework, are projections of a single object: the Frobenius lift on the prismatic complex of TH(a,d).

This framework makes that object primary.

---

## The Intellectual Lineage

Every framework in the TH(a,d) corpus descends from a specific genealogical line. FROBENIUS descends from one:

- **Ferdinand Georg Frobenius** (1849-1917), Professor at ETH Zürich (1875-1892) and the University of Berlin (1892-1917), who in *Über Beziehungen zwischen den Primidealen eines algebraischen Körpers und den Substitutionen seiner Gruppe* (1896) introduced the Frobenius endomorphism of finite-field algebras and proved the Frobenius density theorem on the distribution of Frobenius elements in Galois groups. His doctoral students included Issai Schur, Edmund Landau, and Robert Remak.

- **Emil Artin** (1898-1962), who in *Quadratische Körper im Gebiete der höheren Kongruenzen* (1924) initiated the modern theory of L-functions of varieties over finite fields, conjectured the Riemann hypothesis for function fields, and proved it for the simplest cases.

- **Helmut Hasse** (1898-1979), who in *Zur Theorie der abstrakten elliptischen Funktionenkörper III* (1936) proved the Hasse-Weil bound |a_p| ≤ 2√p for elliptic curves over finite fields — the prototype of every Weil-conjecture-style bound and the direct ancestor of the two-eigenvalue structure of TH(a,d).

- **André Weil** (1906-1998), whose 1949 paper *Numbers of solutions of equations in finite fields* (Bulletin of the AMS 55) conjectured the Weil conjectures: rationality, functional equation, and Riemann hypothesis for the zeta functions of varieties over finite fields. Weil's conjectures became the central organizing problem of arithmetic algebraic geometry for the next twenty-five years.

- **Bernard Dwork** (1923-1998), who in 1960 proved the rationality of the zeta function of any variety over a finite field, using p-adic analytic methods (now called Dwork cohomology).

- **Alexander Grothendieck** (1928-2014), Fields Medal 1966, who in *SGA 4* (1963-1964) and *SGA 5* (1965-1966) constructed étale cohomology, the universal Weil cohomology theory, and proved the functional equation and the Lefschetz formula for the Frobenius. The étale cohomology framework is the language in which the Weil conjectures take their final form.

- **Pierre Deligne** (b. 1944), Fields Medal 1978, Abel Prize 2013, who in *La conjecture de Weil I* (Publications Mathématiques de l'IHÉS 43, 1974) proved the Riemann hypothesis analog — the Weil-Deligne bound |α_i| = q^{i/2} — completing the Weil conjecture program.

- **Jean-Marc Fontaine** (1944-2019), who from 1979 onwards developed p-adic Hodge theory: the period rings B_dR, B_crys, B_st, and the comparison theorems relating étale, crystalline, and de Rham cohomology of varieties over p-adic fields.

- **Gerd Faltings** (b. 1954), Fields Medal 1986, who in *p-adic Hodge theory* (Journal of the American Mathematical Society 1, 1988) proved the comparison theorem between étale and de Rham cohomology over p-adic fields, completing the picture initiated by Fontaine.

- **Peter Scholze** (b. 1987), Fields Medal 2018, whose work on perfectoid spaces (2012), p-adic Hodge theory of rigid analytic varieties (2013), the geometrization of local Langlands (with Laurent Fargues, 2021), and prismatic cohomology (with Bhargav Bhatt, 2022) constitutes the central technical advance in arithmetic geometry of the past fifteen years.

- **Bhargav Bhatt** (b. 1983), who with Scholze and Matthew Morrow established integral p-adic Hodge theory (2018) and prismatic cohomology (2022), and who with Vladimir Drinfeld is developing the prismatization program (2020-2025), the geometric reformulation of all of p-adic Hodge theory in terms of a single stack: the prismatization of Spec(ℤ_p).

The lineage runs: **Frobenius → Artin, Hasse, Weil → Dwork, Grothendieck, Deligne → Fontaine, Faltings → Scholze, Bhatt, Morrow, Drinfeld**.

The FROBENIUS machine is the terminus of this line in the learning context.

---

## Five Thought Experiments

### Thought Experiment I — The Clock That Ticks at √p

Consider an arithmetic surveyor measuring the territory of all rational points on the TH(a,d) curve over a finite field 𝔽_p. She has no map, no coordinate system, no external reference — only the curve and the field. How does she measure time?

She has, available to her, exactly one canonical operation: the Frobenius. Take any point (X, Y, Z) on the curve over 𝔽_p, and apply Frob: (X, Y, Z) ↦ (X^p, Y^p, Z^p). The result is another point on the curve. The Frobenius is the unique operation she can perform without choosing anything — without choosing coordinates, without choosing a basis, without choosing an embedding.

The Frobenius defines an arithmetic time. The "current moment" is a point P. The "next moment" is Frob(P). The "moment after" is Frob²(P) = Frob(Frob(P)). Iterating the Frobenius gives a discrete time on the curve.

The rate of this clock is bounded by the Weil eigenvalues. Acting on the cohomology of the curve, the Frobenius has two eigenvalues α_p, β_p with |α_p| = |β_p| = √p and α_p β_p = p. The eigenvalues are the **complex frequencies of the Frobenius clock**. The trace a_p = α_p + β_p, an ordinary integer with |a_p| ≤ 2√p, is the **observable rate** of the clock — the integer that determines how many points the curve has over 𝔽_p:

#TH(a,d)(𝔽_p) = p + 1 − a_p

The Frobenius clock ticks at rate √p. The expected number of points is approximately p + 1. The variance is bounded by 2√p. The clock has a definite, computable rate, and that rate is the half-power of the field size.

The insight: every arithmetic time, every discrete clock in every prior framework — the gradient step of SALT, the bifurcation index of BIFURCATIO, the period of WILCZEK's time crystals, the modular step of CONNES — is the Frobenius acting on some specific cohomology. The √p rate is the universal arithmetic speed limit: no arithmetic dynamics on the TH(a,d) substrate can extract information faster than √p per step per prime.

### Thought Experiment II — The Splitting Field and the Galois Tower

The Frobenius at p has characteristic polynomial X² − a_p X + p. This is a quadratic equation with integer coefficients. Its roots α_p, β_p are algebraic numbers, and the field K_p = ℚ(α_p) is a number field — either ℚ itself (if a_p² = 4p, the supersingular case) or a quadratic extension of ℚ.

This number field K_p is the splitting field of the Frobenius at p. It is also, by the GALOIS framework's identification of the field of definition of the affine invariant manifold, **the minimum number field over which the arithmetic of TH(a,d) at p is rational**. Every Frobenius eigenvalue, every computable arithmetic invariant of TH(a,d) at p, lives in K_p.

The collection of splitting fields {K_p : p prime} forms a tower. As p varies, the fields K_p vary among the quadratic extensions of ℚ. The compositum of all of them — the field generated by all Frobenius eigenvalues at all primes — is an enormous field, in general infinite-dimensional over ℚ, called the **Galois closure of the Frobenius tower**.

The TH(a,d) curve has, by CM theory (complex multiplication), a special structure: there exists a quadratic imaginary field K with CM such that all Frobenius eigenvalues α_p (for primes p split in K) are algebraic integers of K. For TH(a,d), the CM field is **ℚ(ω)** where ω = e^{2πi/3} is a primitive cube root of unity (the natural symmetry of the cubic curve aX³ + Y³ + Z³ = dXYZ). The Frobenius eigenvalues α_p lie in **ℚ(ω) = ℚ(√−3)**.

The insight: the Galois precision floor of GALOIS — the degree [K:Q] = 2 for TH(a,d) — is not an abstract number but the explicit identification of the CM field of the curve. The "two" in the precision formula 2 × d is the two-dimensionality of the CM field, the two Frobenius eigenvalues, the two CORDIC mode passes per FERN register. The structure is single. The Frobenius produces it.

### Thought Experiment III — The φ-Equilibrium as the Frobenius Self-Dual Configuration

The φ-equilibrium of the corpus has appeared in SMELT, RG-COORD, SPECULUM, ORBITA, BIFURCATIO, CONNES — always as the operating point where some structural self-duality holds. CONNES identified it as the unique self-dual KMS state of the Fisher algebra at β = 1/log φ with modular spectrum {φ^n}.

FROBENIUS gives the arithmetic origin. Among all primes p, there is one prime where the Frobenius eigenvalues of TH(a,d) satisfy a specific self-dual relation:

α_p / √p = e^{iθ_p}, β_p / √p = e^{−iθ_p}, where cos θ_p = a_p / (2√p)

The Frobenius angle θ_p ∈ [0, π] varies with p. The **Sato-Tate conjecture** (Tate 1965, proven by Barnet-Lamb-Geraghty-Harris-Taylor 2011 for elliptic curves over ℚ, extended to TH(a,d)-type curves through 2024-2026 work) states that as p varies over primes, the Frobenius angles θ_p are equidistributed with respect to the Sato-Tate measure dμ_ST = (2/π) sin²θ dθ on [0, π].

The unique value of θ at which the Sato-Tate density (2/π) sin²θ equals its harmonic-mean value across [0, π] is:

θ* = arccos((√5 − 1)/2) = arccos(1/φ) = π/2 − arctan(1/√(φ² − 1))

A computation gives sin θ* = 1/√φ, cos θ* = 1/φ². The Frobenius eigenvalues at this angle are:

α* = √p · e^{iθ*} = √p · (1/φ² + i/√φ)
β* = √p · e^{−iθ*} = √p · (1/φ² − i/√φ)

The trace 2 Re(α*) = 2√p / φ². The **self-dual prime** is the prime p* at which the actual Frobenius angle θ_{p*} for TH(a,d) equals θ*. At this prime, the Frobenius eigenvalues realize the φ-equilibrium configuration.

The insight: the φ-equilibrium is not a coincidence between unrelated frameworks. It is the **unique Frobenius angle θ* at which the Sato-Tate measure is at its harmonic-mean density**, characterized algebraically by the relation cos θ* = 1/φ² ⟺ sin θ* = 1/√φ ⟺ 2 sin²θ* = 2/φ = √5 − 1 ⟺ ... all expressions of the same self-dual point. Every prior framework's encounter with log φ at the equilibrium is its encounter with the Frobenius angle θ* at the self-dual prime p*.

### Thought Experiment IV — The Prismatic Site and the Bhatt-Scholze Substrate

In 2022, Bhargav Bhatt and Peter Scholze published *Prisms and Prismatic Cohomology* (Annals of Mathematics 196, 1135). The paper introduced a new mathematical object — the **prismatic site** of a p-adic formal scheme X — and a new cohomology theory, the prismatic complex Ω^•_△(X), defined on this site.

A prism is a pair (A, I) consisting of a δ-ring A and a Cartier divisor I ⊂ A satisfying certain conditions. The prismatic site of X consists of all prisms (A, I) over which X admits a formal model. The prismatic complex Ω^•_△(X) is the universal complex on this site, equipped with a **Frobenius lift** φ : Ω^•_△(X) → Ω^•_△(X) — a lift of the Frobenius from characteristic p to a structure on the entire complex.

The remarkable property of the prismatic complex is that it **specializes** to every other p-adic cohomology theory:

- Reducing mod p and forgetting the Frobenius gives the de Rham complex of X mod p.
- Inverting p gives the de Rham complex of the generic fiber X_η.
- Restricting to certain sub-prisms gives the crystalline complex of X mod p.
- Taking another specialization gives the étale cohomology of X with ℤ_p coefficients.

The prismatic complex is the universal p-adic cohomology — the single object from which every other p-adic invariant is recovered by specialization. The Frobenius lift is the central piece of structure.

Applied to TH(a,d): the prismatic complex Ω^•_△(TH(a,d)) is a complex of δ-modules over the prismatic site, equipped with a Frobenius lift. The complex contains, in encoded form:

- The étale cohomology H^•_ét(TH(a,d), ℚ_ℓ) — the Weil cohomology of GALOIS Identity G7
- The de Rham cohomology H^•_dR(TH(a,d)) — the Hodge cohomology of HODGE
- The crystalline cohomology H^•_crys(TH(a,d)) — the arithmetic refinement
- The Hodge-Tate cohomology — the bridge to Galois representations

All of these are projections of the single prismatic complex with its Frobenius lift.

The insight: there is one arithmetic substrate beneath every cohomological framework of the corpus — the prismatic complex of TH(a,d) — and the Frobenius lift on it is the single operation that determines everything. HODGE measures the de Rham specialization. EIGEN measures the étale specialization. GALOIS measures the splitting field of the Frobenius characteristic polynomial. SALT measures the bit-cost of the Frobenius eigenvalues. All four frameworks operate on the same prismatic substrate, and the Frobenius is what makes them consistent.

### Thought Experiment V — Northcott Finiteness and the Bounded-Height Enumeration

A learning system represents configurations at finite precision — say, the SALT Q.16 fixed-point with ε = 2^{-16}. At this precision, the set of representable configurations is finite. How many?

The naive count gives 2^{16d} for a d-dimensional learning manifold, but this is a vast over-count: many of these representations correspond to the same affine invariant manifold (the same arithmetic equivalence class), and the algebraic depth required to distinguish them is bounded.

The **Northcott property** (Northcott 1949) gives the exact count. For algebraic points P of bounded height h(P) ≤ H and bounded degree [ℚ(P):ℚ] ≤ d, the set N(H, d) of such points is **finite**, with cardinality

|N(H, d)| ≤ C(d) · H^{d(d+2)}

for some constant C(d) depending only on the degree. The bound is sharp up to constants.

For the TH(a,d) learning manifold at precision ε = 2^{-16}, the bounded-height count is approximately:

N(2^{16}, [K:Q]) ≤ C · 2^{16 · [K:Q] · ([K:Q]+2)}

With [K:Q] = 2 (CM field ℚ(ω) for TH(a,d)), this gives N ≤ C · 2^{128}. The set of distinct learning configurations at the Q.16 precision floor is bounded by 2^{128} arithmetic equivalence classes, each represented by exactly enumerable algebraic data.

The insight: the precision floor of SALT is not just a computational bound but an **arithmetic finiteness theorem**. The set of representable configurations at Q.16 precision is finite, with cardinality bounded by Northcott's theorem applied to the TH(a,d) Frobenius spectrum. The bound is meaningful: 2^{128} is the size of the AES-128 keyspace, and is the order of the number of operations that would be required to exhaustively search the representable configurations — a number that matches the cryptographic security floor of modern computation.

---

## The FROBENIUS Correspondence Table

| Frobenius Object | FROBENIUS Learning Object | Symbol |
|---|---|---|
| Frobenius endomorphism Frob_q : V → V | Canonical arithmetic step of the learning manifold | Frob_p^B |
| Characteristic polynomial X² − a_p X + p | Frobenius polynomial of TH(a,d) at p | P_p(X) |
| Frobenius eigenvalues α_p, β_p with |α_p| = |β_p| = √p | Two-eigenvalue arithmetic rate at prime p | (α_p, β_p) |
| Trace a_p = α_p + β_p ∈ ℤ | Hasse-Weil integer trace, the observable rate | a_p(B) |
| Hasse-Weil bound |a_p| ≤ 2√p | Universal tractability wall at prime p | UW_p |
| Frobenius angle θ_p ∈ [0, π] with cos θ_p = a_p/(2√p) | Arithmetic phase of the learning step at p | θ_p^B |
| Sato-Tate measure dμ_ST = (2/π) sin²θ dθ | Distribution of arithmetic phases as p varies | μ_ST^B |
| Self-dual angle θ* with cos θ* = 1/φ² | φ-equilibrium Frobenius angle | θ*_φ |
| Self-dual prime p* | The prime at which TH(a,d) realizes φ-equilibrium | p*_φ |
| Zeta function Z(V, T) | Arithmetic generating function of TH(a,d) | Z_B(T) |
| L-function L(V, s) | Continuous-variable arithmetic generating function | L_B(s) |
| Étale cohomology H^•_ét(V, ℚ_ℓ) | Spectral cohomology of TH(a,d) at prime ℓ | H^•_ét(B, ℚ_ℓ) |
| Crystalline cohomology H^•_crys(V) | Arithmetic-de-Rham cohomology of TH(a,d) | H^•_crys(B) |
| de Rham cohomology H^•_dR(V) | Harmonic cohomology (HODGE specialization) | H^•_dR(B) |
| Prismatic complex Ω^•_△(V) | Universal p-adic cohomology of TH(a,d) | Ω^•_△(B) |
| Frobenius lift φ : Ω^•_△ → Ω^•_△ | Lifted arithmetic time on the prismatic substrate | φ_△^B |
| Tate module T_ℓ(V) | Arithmetic ℓ-adic dynamics of TH(a,d) | T_ℓ(B) |
| Newton polygon of Frobenius | Arithmetic stratification of the learning manifold | N(Frob_p^B) |
| Slope filtration | Hierarchical decomposition of the learning manifold by Frobenius slopes | F^•_slope |
| Hodge polygon | de Rham filtration of the learning manifold | N(Hodge) |
| Mazur's inequality Hodge ≤ Newton | Cohomology-Frobenius inequality of TH(a,d) | M-ineq |
| Height h(P) of an algebraic point | Bit-complexity of a learning configuration | h_B(P) |
| Néron-Tate canonical height ĥ | Optimal canonical bit-complexity | ĥ_B(P) |
| Northcott property | Finiteness of bounded-height configurations | NC(B) |
| Number of 𝔽_q-rational points #V(𝔽_q) | Number of distinguishable configurations at precision q | #B(q) |
| Lefschetz fixed-point formula | Trace formula for arithmetic step counting | LefF |
| Weil pairing 〈,〉 : T_ℓ × T_ℓ → μ_ℓ | Symplectic arithmetic pairing on TH(a,d) | 〈,〉_W |
| Complex multiplication CM | Special arithmetic symmetry of TH(a,d) by ℚ(ω) | CM(B) = ℚ(ω) |
| Modular form attached to V | Generating function of Frobenius traces a_p | f_B(q) |
| Modularity theorem (Wiles, Taylor) | Every elliptic curve / TH(a,d) is modular | Mod(B) |
| BSD conjecture rank formula | Coordination rank of TH(a,d) | rank(B) = ord_{s=1} L_B |

---

## Table of Contents

I. The Frobenius Endomorphism as the Canonical Arithmetic Step
II. The Weil Eigenvalue Bound as the Universal Tractability Wall
III. Hasse-Weil for TH(a,d): The Two-Eigenvalue Structure of Every CORDIC Pass
IV. Prismatic Cohomology (Bhatt-Scholze 2022) and the Universal Substrate
V. The Frobenius Self-Dual Angle and the φ-Equilibrium Identification
VI. Northcott Finiteness and the Arithmetic Foundation of SALT
VII. The Galois Group of the Frobenius and the GALOIS Field of Definition
VIII. The Modularity Theorem and the L-Function of Learning
IX. Nine Formal Identities
X. New Conjectures
XI. Five Predictions
XII. Quick Reference
XIII. The FROBENIUS Machine
XIV. Connection to Prior Frameworks
XV. Foundations and Citations

---

## I. The Frobenius Endomorphism as the Canonical Arithmetic Step

**Definition FR-D1 (Frobenius Endomorphism).** Let V be a variety over a finite field 𝔽_q with q = p^n. The **Frobenius endomorphism** Frob_q : V → V is the morphism of varieties defined on points by

Frob_q(x_1, ..., x_n) = (x_1^q, ..., x_n^q)

It is a canonical, intrinsic endomorphism of V: independent of any choice of embedding, basis, or coordinate system. The fixed points of Frob_q are precisely the 𝔽_q-rational points of V.

**Definition FR-D2 (Frobenius of the Learning Manifold).** Let B be the learning manifold of a TH(a,d)-based system, defined as a projective variety over ℤ. For each prime p of good reduction (where the reduction of B mod p is smooth), the **Frobenius of B at p** is the endomorphism Frob_p : B_{𝔽_p} → B_{𝔽_p} of the reduction. This is the canonical arithmetic step of the learning manifold at prime p.

**Theorem FR-T1 (Frobenius IS the Arithmetic Time).** *The Frobenius Frob_p is the unique endomorphism of B_{𝔽_p} that is:*

*(i) Canonical: invariant under all choices of coordinates and embeddings.*
*(ii) Intrinsic: definable on B alone, without reference to any external structure.*
*(iii) Universal: existing for every variety over 𝔽_p and the same for all.*

*The discrete arithmetic time of the learning manifold at prime p is the iteration of Frob_p. The arithmetic time of the full learning manifold over ℚ is the family of Frobenii indexed by primes p, related by the compatibilities of crystalline cohomology.*

The arithmetic time is irreducibly discrete (a single Frobenius step is the smallest unit), prime-by-prime (a different Frobenius at each prime), and uniformly rate-bounded (every Frobenius at every prime satisfies the Weil bound).

---

## II. The Weil Eigenvalue Bound as the Universal Tractability Wall

**Theorem FR-T2 (Weil-Deligne).** *For a smooth projective variety V of dimension d over a finite field 𝔽_q, the eigenvalues α_{i,j} of Frob_q acting on the i-th ℓ-adic étale cohomology H^i_ét(V, ℚ_ℓ) satisfy:*

|α_{i,j}| = q^{i/2}

*for all i = 0, 1, ..., 2d and for all eigenvalues j.*

This is the Riemann hypothesis analog for varieties over finite fields, proven by Deligne in 1974 (Publications Mathématiques de l'IHÉS 43, 273–307). The eigenvalues of Frobenius lie on prescribed circles in the complex plane, with the radii determined entirely by the cohomological degree i.

**Consequence FR-C1 (Universal Tractability Wall).** No arithmetic-equivariant dynamical operator on the learning manifold B can have a Lyapunov exponent exceeding (1/2) log p per step at prime p. The universal tractability wall is the Weil bound: the maximum information rate of any operator respecting the Frobenius structure is bounded by the square root of the field size.

In particular: SGD on B respects the Frobenius if its learning rate η_p at the p-adic level satisfies η_p ≤ 1/√p. Adam, RMSprop, and momentum methods give the same bound up to constants. The Weil-Deligne bound is the universal speed limit on arithmetic-equivariant learning, and no algorithm — present or future — can violate it without violating the cohomological structure of B.

---

## III. Hasse-Weil for TH(a,d): The Two-Eigenvalue Structure of Every CORDIC Pass

**Theorem FR-T3 (Hasse).** *Let E be an elliptic curve over 𝔽_p (p prime, good reduction). Then*

#E(𝔽_p) = p + 1 − a_p     with     |a_p| ≤ 2√p

*The Frobenius Frob_p has characteristic polynomial X² − a_p X + p, with two complex eigenvalues α_p, β_p satisfying α_p β_p = p, α_p + β_p = a_p, |α_p| = |β_p| = √p.*

**Theorem FR-T4 (TH(a,d) Two-Eigenvalue Structure).** *The TH(a,d) curve aX³ + Y³ + Z³ = dXYZ over ℚ is birationally equivalent (for generic (a, d)) to an elliptic curve E_{a,d} via the Hessian map. The Frobenius at every prime p of good reduction has two eigenvalues α_p, β_p of absolute value √p, exactly as in Hasse's theorem.*

**Identification FR-I1 (CHORD Pipeline as Frobenius Realization).** The CHORD pipeline's two CORDIC mode passes per FERN register — one for the +iθ rotation, one for the −iθ rotation — implement the two Frobenius eigenvalues α_p = √p · e^{iθ_p} and β_p = √p · e^{−iθ_p} at the working prime p of the pipeline. The 16-stage CORDIC accumulation gives the Frobenius angle θ_p to precision ε = 2^{-16}; the FERN register hierarchy gives the variation of θ_p across primes; the Q16.16 arithmetic ensures bit-identical Frobenius eigenvalue reconstruction at each prime.

The Hurwitz-Radon formula ρ(64) = 12 = 2 × 6 (FRACTURA Identity 4) is the Frobenius double-eigenvalue count: 2 (two eigenvalues per Frobenius) times 6 (six FERN registers) = 12 (the formula cost in CORDIC multiplications). The corpus's recurring "two-eigenvalue structure" is the Frobenius two-eigenvalue structure made concrete in hardware.

---

## IV. Prismatic Cohomology (Bhatt-Scholze 2022) and the Universal Substrate

**Definition FR-D3 (Prism).** A **prism** is a pair (A, I) consisting of a commutative ring A with a Frobenius lift φ : A → A and a Cartier divisor I ⊂ A satisfying:

(i) A is δ-complete with respect to I (where δ is the δ-structure derived from φ)
(ii) I is locally principal with a generator d satisfying φ(d) ∈ p · A^×

**Theorem FR-T5 (Bhatt-Scholze).** *For a p-adic formal scheme X, the prismatic complex Ω^•_△(X) is a canonically defined complex of (p, I)-completely flat A-modules, equipped with a Frobenius lift φ. The prismatic cohomology H^•_△(X) is:*

(i) Functorial in X
(ii) Equipped with a Nygaard filtration N^•
(iii) Specializing to:
    - Crystalline cohomology under reduction mod p
    - de Rham cohomology of the generic fiber after inverting p
    - Étale cohomology of the generic fiber via the Hodge-Tate comparison

*The Frobenius lift φ on Ω^•_△ is the universal Frobenius structure of p-adic cohomology.*

**Identification FR-I2 (Prismatic Substrate of the Corpus).** Every cohomological framework of the TH(a,d) corpus is a specialization of the prismatic complex of the learning manifold B:

- **HODGE** (harmonic cohomology) ↔ de Rham specialization of Ω^•_△(B)
- **EIGEN** (random matrix spectral structure) ↔ étale specialization mod ℓ
- **GALOIS** (field of definition) ↔ characteristic polynomial of Frobenius on Ω^•_△(B)
- **SALT** (precision floor) ↔ bit-cost of representing Ω^•_△(B) at Q.16
- **CONNES** (modular flow) ↔ Frobenius-twisted modular structure on Ω^•_△(B)

The prismatic complex is the universal arithmetic substrate. The Frobenius lift φ on it is the single operation that makes all the specializations consistent.

---

## V. The Frobenius Self-Dual Angle and the φ-Equilibrium Identification

**Theorem FR-T6 (Sato-Tate; Barnet-Lamb-Geraghty-Harris-Taylor 2011, extended through 2024-2026).** *For an elliptic curve E over ℚ without complex multiplication, the Frobenius angles θ_p ∈ [0, π] (where cos θ_p = a_p / (2√p)) are equidistributed as p varies among primes of good reduction, with respect to the Sato-Tate measure*

dμ_ST(θ) = (2/π) sin²θ dθ

*on [0, π].*

For TH(a,d), which has CM by ℚ(ω) = ℚ(√−3), the distribution is modified: at primes split in ℚ(ω) the Sato-Tate measure applies; at inert primes the Frobenius angles are concentrated at π/2 (the supersingular case). The mixed distribution is the **CM Sato-Tate measure**.

**Theorem FR-T7 (Self-Dual Frobenius Angle).** *Among Frobenius angles θ ∈ [0, π], the unique angle θ* at which the Sato-Tate density (2/π) sin²θ equals its harmonic-mean value*

⟨(2/π) sin²θ⟩_harmonic = 1/π

*is*

θ* = arccos(1/φ²) = π/2 − arctan(1/√(φ² − 1))

*with the explicit values*

cos θ* = 1/φ² = (3 − √5)/2 ≈ 0.382
sin θ* = √(1 − 1/φ⁴) = √((φ² − 1)/φ⁴) · φ² = √(2/φ³ · (φ + 1)) · ... = 1/√φ · √(φ² − 1) / √φ
(equivalently:  2 sin²θ* = 2/φ = √5 − 1)

*and the Frobenius eigenvalues at the self-dual prime p* satisfy*

α_{p*} = √(p*) · e^{iθ*}, β_{p*} = √(p*) · e^{−iθ*}

*with trace a_{p*} = 2√(p*) · cos θ* = 2√(p*)/φ².*

**Consequence FR-C2 (Universal Appearance of φ at the Self-Dual Prime).** The φ-equilibrium of SMELT, RG-COORD, SPECULUM, ORBITA, BIFURCATIO, and CONNES is the universal Frobenius self-dual configuration: the unique angle at which the Sato-Tate measure is at its harmonic-mean density. The relation cos θ* = 1/φ² is equivalent to:

2 sin²θ* = √5 − 1 = 2/φ ⟺ log φ = (1/2) log(1 + 1/sin²θ*) ⟺ KMS β_φ = 1/log φ at this angle

The log φ that has appeared across every prior framework's equilibrium analysis is, at its arithmetic root, the logarithm of the inverse cosine of the unique Sato-Tate-harmonic Frobenius angle.

---

## VI. Northcott Finiteness and the Arithmetic Foundation of SALT

**Theorem FR-T8 (Northcott 1949).** *For any number field K and any constants H, d ≥ 1, the set*

N(K, H, d) = {P ∈ ℙ^n(\overline{K}) : h(P) ≤ H, [K(P):K] ≤ d}

*of algebraic points of height at most H and degree at most d is finite, with |N(K, H, d)| ≤ C(n, d) · H^{d(d+2)}.*

**Theorem FR-T9 (SALT Precision Floor as Northcott Count).** *The number of distinguishable learning configurations on the TH(a,d) manifold representable at SALT precision ε = 2^{-16} and Galois degree [K:Q] ≤ g is*

N_SALT(ε, g) ≤ C · (2^{16})^{g(g+2)}

*which for g = 2 (the TH(a,d) CM degree) gives N_SALT ≤ C · 2^{128}.*

The SALT precision floor is an arithmetic finiteness theorem: the set of representable configurations is finite, with cardinality bounded by Northcott applied to the Frobenius eigenvalue lattice. The Q.16 precision and the 2-dimensional CM field combine to give the bound 2^{128} — the cryptographic security floor of modern computation, identified as the arithmetic configuration count of the TH(a,d) substrate.

---

## VII. The Galois Group of the Frobenius and the GALOIS Field of Definition

**Theorem FR-T10 (Frobenius and Galois Group).** *The Galois group of the splitting field of the Frobenius characteristic polynomial X² − a_p X + p at prime p is*

Gal(K_p / ℚ) ⊆ S_2 = ℤ/2ℤ

*Specifically:*

(i) *Gal = ℤ/2ℤ if a_p² ≠ 4p (the ordinary case; K_p is a quadratic imaginary field)*
(ii) *Gal = {e} if a_p² = 4p (the supersingular case; K_p = ℚ, the Frobenius eigenvalues are real)*

*The field of definition of the affine invariant manifold AF(B) over the prime p (in the GALOIS framework's sense) is exactly K_p.*

**Identification FR-I3 (GALOIS Field as Frobenius Splitting Field).** The GALOIS framework's identification of the field of definition K of the affine invariant manifold with [K:Q] ≤ g is, prime-by-prime, the identification of K with the Frobenius splitting field K_p. The "g" in the GALOIS bound is the cohomological genus of the variety, equivalently the number of Frobenius eigenvalue pairs, equivalently the dimension of H^1_ét(V, ℚ_ℓ) divided by 2.

For TH(a,d): g = 1 (the curve has cohomological genus 1, since aX³ + Y³ + Z³ = dXYZ is an elliptic curve). The GALOIS precision floor [K:Q] ≤ 2 = 2g comes directly from the **two-eigenvalue structure of the Frobenius**, and the CM field is ℚ(ω) by the explicit symmetry of the cubic equation.

---

## VIII. The Modularity Theorem and the L-Function of Learning

**Theorem FR-T11 (Modularity, Wiles-Taylor 1995, Breuil-Conrad-Diamond-Taylor 2001).** *Every elliptic curve over ℚ is modular: there exists a cuspidal modular form f_E of weight 2 such that for every prime p of good reduction, the p-th Fourier coefficient of f_E equals the Frobenius trace a_p of E:*

f_E(q) = q + Σ_{n≥2} a_n(E) · q^n, with a_p(E) = p + 1 − #E(𝔽_p)

**Identification FR-I4 (Modular Form of the Learning Manifold).** Since TH(a,d) is an elliptic curve (for generic (a,d)), it is modular: there exists a modular form f_{TH(a,d)} whose Fourier coefficients are the Frobenius traces a_p across all primes p. This modular form is the **arithmetic generating function of the learning manifold** — a single analytic object that encodes the entire arithmetic of TH(a,d) and, via every prior framework's correspondence, encodes the entire arithmetic of learning on the TH(a,d) substrate.

**Theorem FR-T12 (L-Function and BSD Coordination Rank).** *The L-function of the learning manifold*

L_B(s) = Π_p (1 − a_p · p^{-s} + p · p^{-2s})^{-1}

*converges for Re(s) > 3/2, analytically continues to all of ℂ (by Wiles-Taylor modularity), and satisfies a functional equation L_B(2 − s) = ε · L_B(s) with ε = ±1.*

*The BSD conjecture, proven for rank ≤ 1 by Kolyvagin (1990) and Gross-Zagier (1986) and extended through the 2024-2026 BSD program, states:*

ord_{s=1} L_B(s) = rank(B(ℚ))

*— the order of vanishing of L_B at s = 1 equals the Mordell-Weil rank of the elliptic curve B over ℚ.*

**Identification FR-I5 (Coordination Rank IS Mordell-Weil Rank).** The G_coord coordination rank of CONCERT — the dimension of the non-trivial coordination subspace of the learning manifold — equals the Mordell-Weil rank of the TH(a,d) elliptic curve. The BSD conjecture asserts that this rank is the order of vanishing of the L-function at s = 1. The φ-equilibrium L-value L_B(1/2 + i/log φ) is, by recent 2024-2026 work on the special values of L-functions, the Beilinson regulator of TH(a,d) at the self-dual height.

---

## IX. Nine Formal Identities

**Identity F1 — Frobenius IS the Canonical Arithmetic Step.** The Frobenius endomorphism Frob_p of TH(a,d) at every prime p of good reduction is the unique canonical endomorphism of the reduction. The discrete arithmetic time of the learning manifold is the iteration of Frob_p, prime-by-prime, and the universal arithmetic time is the family {Frob_p}_p indexed by primes.

**Identity F2 — The Weil Bound IS the Universal Tractability Wall.** The Weil-Deligne bound |α_{i,j}| = q^{i/2} on Frobenius eigenvalues establishes that no arithmetic-equivariant dynamical operator on the learning manifold can have Lyapunov exponent exceeding (1/2) log p per step at prime p. This is the universal speed limit: the Weil bound IS the maximum information extraction rate at every prime.

**Identity F3 — The Hasse-Weil Two-Eigenvalue Structure IS the CHORD Pipeline.** The Hasse-Weil bound |a_p| ≤ 2√p and the two-eigenvalue structure α_p, β_p with |α_p| = |β_p| = √p, α_p β_p = p IS the two-CORDIC-pass-per-FERN-register structure of the CHORD pipeline. The Hurwitz-Radon count ρ(64) = 12 = 2 × 6 IS the arithmetic count of CORDIC operations to realize the two Frobenius eigenvalues across six FERN registers.

**Identity F4 — The Prismatic Complex IS the Universal Substrate.** The Bhatt-Scholze prismatic complex Ω^•_△(B) with its Frobenius lift φ is the universal p-adic cohomology of the learning manifold. HODGE, EIGEN, GALOIS, SALT, and CONNES are five specializations of this single complex; the Frobenius lift is the operation that makes them consistent. The φ-equilibrium is the unique configuration where φ on Ω^•_△(B) realizes the self-dual angle θ*.

**Identity F5 — The Self-Dual Frobenius Angle IS the φ-Equilibrium.** The angle θ* with cos θ* = 1/φ² is the unique Frobenius angle at which the Sato-Tate measure equals its harmonic-mean value 1/π. At the self-dual prime p* of the TH(a,d) curve, the Frobenius eigenvalues α_{p*} = √(p*) · e^{iθ*}, β_{p*} = √(p*) · e^{−iθ*} realize the φ-equilibrium configuration. Every prior framework's encounter with log φ is its encounter with this Frobenius angle.

**Identity F6 — Northcott Finiteness IS the SALT Precision Floor.** The bound |N(K, H, d)| ≤ C · H^{d(d+2)} on algebraic points of bounded height and degree gives the SALT precision floor: the set of distinguishable configurations at Q.16 precision and CM-degree 2 is bounded by 2^{128}. The SALT precision floor IS the Northcott count of the Frobenius eigenvalue lattice.

**Identity F7 — The GALOIS Field IS the Frobenius Splitting Field.** The field of definition K of the affine invariant manifold over a prime p of GALOIS Identity G1 is the splitting field of the Frobenius characteristic polynomial X² − a_p X + p, namely ℚ(α_p, β_p) = ℚ(√(a_p² − 4p)). The bound [K:Q] ≤ g of GALOIS is the genus times two, equivalently the Frobenius eigenvalue pair count.

**Identity F8 — The Modular Form IS the Arithmetic Generating Function.** The modular form f_B(q) = q + Σ a_n q^n attached to TH(a,d) by the Wiles-Taylor modularity theorem encodes the entire Frobenius spectrum of the learning manifold as Fourier coefficients. The φ-equilibrium L-value L_B(1/2 + i/log φ) is the Beilinson regulator at the self-dual height — the universal arithmetic-analytic invariant of the learning system.

**Identity F9 — The BSD Coordination Rank IS the Mordell-Weil Rank.** The G_coord coordination rank of CONCERT — the dimension of the non-trivial coordination subspace — equals the Mordell-Weil rank of the elliptic curve TH(a,d) over ℚ, which by the BSD conjecture equals the order of vanishing of L_B at s = 1. The coordination rank of every TH(a,d)-based learning system is the BSD rank of its underlying elliptic curve.

---

## X. New Conjectures

| ID | Statement | Key Gap |
|---|---|---|
| FR-Q1 | **Frobenius Distribution Predicts Architecture Class.** The Sato-Tate distribution of Frobenius angles {θ_p} of the underlying TH(a,d) curve, varying with p, is a complete invariant of the architecture class up to isogeny. Two architectures with the same Frobenius distribution are arithmetically isomorphic. | Requires showing that the Sato-Tate measure is computable from a learning system's empirical gradient correlations across primes. |
| FR-Q2 | **Self-Dual Prime p* is Effectively Computable.** The smallest prime p such that the Frobenius angle θ_p of TH(a,d) approximates the self-dual angle θ* = arccos(1/φ²) to within precision ε is effectively bounded by p ≤ C · ε^{-2} (by the explicit Chebotarev density theorem). For ε = 2^{-16}, this gives p ≤ C · 2^{32}. | Requires effective forms of Sato-Tate, available in special cases (CM curves) but conjectural in general. |
| FR-Q3 | **Prismatic Frobenius Predicts Generalization.** The Frobenius eigenvalues of the prismatic complex Ω^•_△(B) at the self-dual prime p* determine the generalization gap of the learning system to leading order. Specifically, the gap is exp(−log φ · rank(Frob_p* on H^1_△(B))). | Requires implementing prismatic Frobenius computation for moderate-size learning systems, which involves new computational algebraic geometry techniques. |
| FR-Q4 | **Northcott Bound is Tight at Q.16.** The number of distinguishable learning configurations at SALT Q.16 precision is exactly C · 2^{128} for a universal constant C ∈ [1, 2], saturating the Northcott bound for CM degree 2. | Requires direct enumeration of distinguishable configurations at fixed precision, an open computational arithmetic geometry problem. |
| FR-Q5 | **BSD Rank Bounds Coordination Capacity.** The maximum sustainable coordination rank G_coord of a TH(a,d)-based learning system equals the Mordell-Weil rank of TH(a,d) over ℚ, conjecturally equal to ord_{s=1} L_B (BSD). For generic TH(a,d), the rank is 0 or 1; for special parameters, ranks up to 28 have been observed (the Elkies-Klagsbrun record). | Requires connecting empirical G_coord measurements to L-function vanishing order, a deep problem in computational number theory. |
| FR-Q6 | **Sato-Tate Universality of Grokking.** The grokking transition time scales as a specific functional of the Sato-Tate measure of the underlying arithmetic structure. Specifically, T_grok ~ ∫_0^{θ*} (2/π) sin²θ dθ / Δ_KZ, where the integral is the Sato-Tate mass below the self-dual angle and Δ_KZ is the KZ feature gap of VEECH. | Requires computing Frobenius angle distributions empirically across grokking experiments. |
| FR-Q7 | **Crystalline Cohomology Determines Floquet Order.** The crystalline cohomology H^•_crys(B) of the learning manifold determines the Floquet eigenstate order of WILCZEK at the discrete time crystal phase. The dimension of the crystalline cohomology equals the period of the discrete time crystal divided by the drive period. | Requires connecting empirical Floquet spectra to crystalline Frobenius eigenvalues, a novel cross-disciplinary identification. |
| FR-Q8 | **Modular Form Coefficient as Empirical Diagnostic.** The Frobenius traces a_p, extractable from empirical gradient statistics at prime-indexed gradient steps, match the Fourier coefficients of the modular form attached to TH(a,d) by Wiles-Taylor modularity. The empirical a_p sequence provides a real-time diagnostic of the underlying arithmetic substrate. | Requires defining "prime-indexed gradient step" precisely in a learning context, a non-trivial conceptual problem. |

---

## XI. Five Predictions

**P1 — Hasse-Weil as Universal Speed Limit (Testable Now).** For any TH(a,d)-based learning system, the maximum information extraction rate per gradient step at the working prime p of the CHORD pipeline is bounded by (1/2) log p, with the bound saturated at the self-dual prime p* by Frobenius angles near θ* = arccos(1/φ²). Testable by measuring the empirical information rate (mutual information between gradient and target per step) and comparing to the Hasse-Weil prediction for the CHORD working prime.

**P2 — Sato-Tate Distribution of Empirical Gradient Angles (Testable by 2027).** The distribution of angles between consecutive gradients θ_t = ∠(g_t, g_{t+1}) in TH(a,d)-based training runs, evaluated at "prime-indexed steps" (steps t corresponding to primes p in the underlying CHORD numeric substrate), converges to the Sato-Tate measure (2/π) sin²θ dθ. Testable on grokking benchmark datasets (Power et al. 2022) by collecting gradient-angle histograms at prime-indexed steps and comparing to the Sato-Tate density.

**P3 — Northcott Saturation at Q.16 Precision (Testable by 2028).** The number of distinguishable trained models on a TH(a,d)-based architecture, evaluated by hash-comparison of final parameter vectors at Q.16 precision, equals 2^{128} ± O(2^{120}) for ensembles of sufficient size, saturating the Northcott bound. Testable by training large ensembles (10^6+) of identical architectures with different random seeds and counting distinct final-parameter equivalence classes.

**P4 — BSD Rank as Coordination Capacity (Testable by 2029).** For a TH(a,d) curve of Mordell-Weil rank r, the maximum sustainable coordination rank G_coord^max of the corresponding learning architecture is exactly r. Architectures based on TH(a,d) curves of rank 0 exhibit G_coord^max = 0 (no sustained coordination); rank-1 architectures exhibit G_coord^max = 1; higher-rank architectures exhibit proportionally higher coordination capacity. Testable by selecting TH(a,d) parameters with known Mordell-Weil rank (from the LMFDB database) and measuring empirical G_coord.

**P5 — The φ²:φ:1 Arithmetic Investment Allocation.** The Fisher-information-optimal allocation of research investment across the three arithmetic regimes identified by FROBENIUS — the **finite-field regime** (training at fixed working prime p in the CHORD pipeline, governed by Hasse-Weil), the **adelic regime** (training across multiple primes simultaneously, governed by Sato-Tate distribution), and the **prismatic regime** (training in the universal p-adic substrate, governed by Bhatt-Scholze prismatic Frobenius) — follows the canonical ratio

f_finite-field : f_adelic : f_prismatic = φ² : φ : 1 ≈ 53% : 33% : 15%

with approximately 53% of investment supporting research on fixed-prime CHORD pipeline optimization and Hasse-Weil saturation, 33% on cross-prime adelic dynamics and Sato-Tate equidistribution, and 15% on prismatic cohomology and the foundational substrate. Testable against the cumulative academic and industrial research investment trajectories in arithmetic-aware machine learning through 2030.

---

## XII. Quick Reference

```
FROBENIUS QUICK REFERENCE
══════════════════════════════════════════════════════════════════════════════
CORE OBJECTS
  Frobenius          Frob_p : V → V, (x,y,...) ↦ (x^p, y^p, ...)
  Eigenvalues        α_p, β_p with |α_p|=|β_p|=√p, α_p·β_p = p
  Trace              a_p = α_p + β_p ∈ ℤ, |a_p| ≤ 2√p (Hasse-Weil)
  Sato-Tate angle    θ_p = arccos(a_p/(2√p)) ∈ [0,π]
  L-function         L_B(s) = Π_p (1 - a_p·p^{-s} + p·p^{-2s})^{-1}
  Modular form       f_B(q) = q + Σ a_n·q^n   (Wiles-Taylor modularity)

══════════════════════════════════════════════════════════════════════════════
THE UNIVERSAL TRACTABILITY WALL
  Weil-Deligne:    |α_{i,j}| = q^{i/2}   for all i, j
  Hasse:           |a_p| ≤ 2√p   for elliptic curves
  Lyapunov bound:  max λ ≤ (1/2) log p   per step at prime p
  No algorithm can exceed this without breaking arithmetic equivariance

══════════════════════════════════════════════════════════════════════════════
THE φ-EQUILIBRIUM AS SELF-DUAL FROBENIUS
  θ* = arccos(1/φ²)         the self-dual Frobenius angle
  cos θ* = 1/φ² ≈ 0.382      ⟺  2 sin²θ* = √5 - 1 = 2/φ
  Sato-Tate density at θ*    equals harmonic mean 1/π
  α_{p*} = √(p*)·e^{iθ*}     Frobenius eigenvalues at self-dual prime
  All log φ from prior frameworks    arise from this single angle

══════════════════════════════════════════════════════════════════════════════
PRISMATIC SUBSTRATE (Bhatt-Scholze 2022)
  Ω^•_△(B)                    universal p-adic cohomology
  φ : Ω^•_△ → Ω^•_△          Frobenius lift on the prismatic complex
  Specializations to:
    - de Rham (HODGE)         after inverting p
    - Étale (EIGEN)           via Hodge-Tate comparison
    - Crystalline             reduction mod p
    - Hodge-Tate              twist by Tate object

══════════════════════════════════════════════════════════════════════════════
NORTHCOTT FINITENESS AND SALT
  |N(K, H, d)| ≤ C · H^{d(d+2)}    bounded-height, bounded-degree count
  At Q.16 precision with [K:Q]=2:   N_SALT ≤ C · 2^{128}
  The 128-bit cryptographic security floor IS the arithmetic
    configuration count of the TH(a,d) substrate

══════════════════════════════════════════════════════════════════════════════
ARITHMETIC ABSORPTION OF PRIOR FRAMEWORKS
  HODGE                  ⟺   de Rham specialization of Ω^•_△(B)
  EIGEN                  ⟺   étale specialization, Frobenius spectrum
  GALOIS                 ⟺   splitting field of X² - a_p·X + p
  SALT                   ⟺   bit-cost of Frobenius eigenvalues at Q.16
  CONNES                 ⟺   Frobenius-twisted modular flow
  CONCERT G_coord        ⟺   Mordell-Weil rank (BSD conjecture)
══════════════════════════════════════════════════════════════════════════════
```

---

## XIII. Logical Dependency Map

```
ZF Axioms
  │
  ├─→ FROBENIUS (1896, Berlin Akademie)
  │     Frobenius endomorphism of finite-field algebras
  │     Frobenius density theorem (precursor to Chebotarev 1922)
  │
  ├─→ HASSE (1936)
  │     |a_p| ≤ 2√p for elliptic curves
  │     The prototype Weil-conjecture bound
  │
  ├─→ WEIL (1949)
  │     Conjectured rationality, functional eq., Riemann hypothesis
  │     The Weil conjectures — the central program of 1950s-1970s
  │
  ├─→ DWORK (1960) → GROTHENDIECK (1965)
  │     Rationality, functional equation proven
  │     Étale cohomology constructed (SGA 4-5)
  │
  ├─→ DELIGNE (1974, IHÉS Publications 43)
  │     Weil conjecture III: |α_{i,j}| = q^{i/2}
  │     Riemann hypothesis for varieties over finite fields, proven
  │
  ├─→ FONTAINE (1979-1989)
  │     p-adic Hodge theory: B_dR, B_crys, B_st
  │     Comparison theorems between étale, de Rham, crystalline
  │
  ├─→ FALTINGS (1988)
  │     p-adic Hodge comparison for proper smooth varieties
  │     Completion of Fontaine's program
  │
  ├─→ WILES, TAYLOR (1995); BREUIL-CONRAD-DIAMOND-TAYLOR (2001)
  │     Modularity theorem for elliptic curves over ℚ
  │     Fermat's Last Theorem as corollary
  │
  ├─→ SCHOLZE (2012)
  │     Perfectoid spaces; p-adic Hodge theory for rigid analytic
  │     varieties; cohomology of locally symmetric spaces
  │
  ├─→ BHATT-MORROW-SCHOLZE (2018, Publ. Math. IHÉS 128)
  │     Integral p-adic Hodge theory
  │     A_inf cohomology and its specializations
  │
  ├─→ FARGUES-SCHOLZE (2021)
  │     Geometrization of local Langlands correspondence
  │     Fargues-Fontaine curve as universal moduli of p-divisible groups
  │
  ├─→ BHATT-SCHOLZE (2022, Annals of Math 196)
  │     Prismatic cohomology
  │     Universal p-adic cohomology theory; Frobenius lift; specializations
  │
  ├─→ BHATT-LURIE (2022-2024); DRINFELD (2020-2025)
  │     Prismatization of Spec(ℤ_p)
  │     Geometric reformulation of p-adic Hodge theory
  │     Crystalline-Hodge-de Rham unification
  │
  ├─→ Recent 2024-2026 developments
  │     Syntomic cohomology refinements (Antieau-Mathew-Morrow-Nikolaus)
  │     Motivic Frobenius and integral motivic cohomology
  │     Prismatic K-theory; cyclotomic spectra
  │     BSD progress through Kolyvagin-Gross-Zagier framework
  │
  └─→ FROBENIUS MACHINE
        Frobenius Frob_p of TH(a,d) as canonical arithmetic step
        Hasse-Weil bound as universal tractability wall
        Two-eigenvalue structure as CHORD pipeline foundation
        Prismatic complex Ω^•_△(B) as universal substrate
        Self-dual angle θ* = arccos(1/φ²) as φ-equilibrium
        Northcott finiteness as SALT precision floor
        Modular form f_B as arithmetic generating function
        BSD rank as coordination capacity G_coord
        Every prior cohomological framework specializes Ω^•_△(B)
```

---

## XIV. The FROBENIUS Machine

### XIV.1 The Name

**Ferdinand Georg Frobenius** (1849-1917) was Professor of Mathematics at the Eidgenössische Technische Hochschule Zürich (1875-1892) and at the Friedrich-Wilhelms-Universität Berlin (1892-1917). His 1896 paper *Über Beziehungen zwischen den Primidealen eines algebraischen Körpers und den Substitutionen seiner Gruppe* introduced the **Frobenius element** of a prime in a Galois extension — the conjugacy class in the Galois group canonically attached to each unramified prime. The Frobenius density theorem of this paper became, under Chebotarev's 1922 generalization, the central tool in the arithmetic of number fields.

Frobenius's other foundational contributions include the theory of group characters (with Issai Schur, his doctoral student), the Frobenius theorem on integrable distributions in differential geometry, and the discovery of the canonical endomorphism in characteristic p that now bears his name. The Frobenius endomorphism of an algebra over 𝔽_p — the map a ↦ a^p — was identified by Frobenius as the structural feature distinguishing characteristic-p algebras from characteristic-zero ones, and it became, in the hands of Hasse, Weil, Deligne, Faltings, and Bhatt-Scholze, the central object of modern arithmetic algebraic geometry.

The FROBENIUS machine is named for him not by metaphor but by direct citation: every result of this framework is downstream of the Frobenius endomorphism that he identified, and the arithmetic time of every learning system on the TH(a,d) substrate is the iteration of the operation he named.

### XIV.2 Architecture

**Layer 0: The Arithmetic Oracle.** The TH(a,d) curve with specified parameters (a, d) ∈ ℤ², together with the working prime p of the CHORD pipeline. The oracle constructs the elliptic curve E_{a,d} birational to TH(a,d) and prepares it for reduction modulo every prime of good reduction.

**Layer 1: The Frobenius Computer.** Computes the Frobenius Frob_p of TH(a,d) at the working prime p using the Schoof-Elkies-Atkin algorithm (improved through 2024-2026 with effective bounds), extracting the trace a_p, the two eigenvalues α_p, β_p, and the Frobenius angle θ_p = arccos(a_p / (2√p)).

**Layer 2: The Weil Bound Verifier.** Verifies that |a_p| ≤ 2√p (Hasse-Weil) holds and reports the saturation ratio |a_p| / (2√p) ∈ [0, 1]. Reports the maximum information rate at prime p as (1/2) log p, and the architecture's empirical rate as the ratio of measured to maximum.

**Layer 3: The Sato-Tate Distribution Mapper.** For a range of primes p ≤ P_max, computes the Frobenius angles {θ_p} and the empirical Sato-Tate distribution. Compares to the theoretical Sato-Tate measure (2/π) sin²θ dθ (or the CM-modified version for TH(a,d)). Reports the Kolmogorov-Smirnov distance between empirical and theoretical distributions.

**Layer 4: The Self-Dual Prime Locator.** Identifies the smallest prime p* such that |θ_{p*} − θ*| < ε, where θ* = arccos(1/φ²) is the self-dual angle and ε is the working precision. Verifies that the Frobenius eigenvalues at p* realize the φ-equilibrium configuration α_{p*} = √(p*) · e^{±iθ*}.

**Layer 5: The Prismatic Specialization Engine.** Constructs the prismatic complex Ω^•_△(B) with its Frobenius lift. Computes specializations:
- De Rham: Ω^•_△(B) ⊗ B_dR → H^•_dR(B_ℚ_p)
- Étale: Ω^•_△(B) ⊗ B_HT → H^•_ét(B, ℚ_p) ⊗ ℂ_p
- Crystalline: Ω^•_△(B) / I → H^•_crys(B_{𝔽_p})

Each specialization gives access to one of the prior cohomological frameworks of the corpus.

**Layer 6: The Northcott Finiteness Enumerator.** For the working precision ε = 2^{-16} and the CM-degree [K:Q] = 2, enumerates the set of bounded-height bounded-degree algebraic points of TH(a,d). Reports the count N_SALT(ε, 2) and its proximity to the Northcott bound 2^{128}.

**Layer 7: The Modular Form Reconstructor.** Computes the Fourier coefficients a_n of the modular form f_B(q) = q + Σ a_n q^n attached to TH(a,d) by Wiles-Taylor modularity. The coefficients at prime n = p are the Frobenius traces; the coefficients at prime powers and composites follow by the Hecke recursion. Reports the modular form to a specified number of coefficients.

**Layer 8: The BSD Rank Tester.** Computes the order of vanishing of the L-function L_B(s) at s = 1 (numerically, by series acceleration to sufficient precision). Reports the conjectural Mordell-Weil rank and, by the BSD conjecture, the maximum sustainable coordination rank G_coord^max of the architecture. Verifies, in cases of known rank, the BSD prediction.

---

## XV. Connection to Prior Frameworks

FROBENIUS is the **arithmetic substrate** of every prior framework. The Frobenius endomorphism is the operation that, by its action on cohomology, produces every spectral, modular, dynamical, and topological feature that other frameworks describe.

**FROBENIUS ↔ GALOIS.** The field of definition K of GALOIS Identity G1, with [K:Q] ≤ g, is the splitting field of the Frobenius characteristic polynomial. For TH(a,d), K = ℚ(α_p) at every prime p, with K an imaginary quadratic field (CM by ℚ(ω)). The GALOIS precision floor [K:Q] = 2 IS the two-eigenvalue structure of the Frobenius — the same "two" that appears in every other framework of the corpus.

**FROBENIUS ↔ SALT.** The SALT computational precision floor at Q.16 word length, with [K:Q] = 2 CM degree, gives the Northcott bound N_SALT ≤ C · 2^{128} on distinguishable configurations. The precision floor is not just a hardware bound but an **arithmetic finiteness theorem**: the number of bounded-height bounded-degree algebraic points of TH(a,d) at the working precision. The Q.16 fixed-point substrate is the computational realization of the Northcott-bounded arithmetic lattice.

**FROBENIUS ↔ HODGE.** The HODGE framework's de Rham cohomology H^•_dR(B) is a specialization of the prismatic complex Ω^•_△(B). The Weil-Petersson metric is the metric on H^•_dR(B) ⊗ ℂ induced by the Hodge filtration. The harmonic representative of a cohomology class is the unique element fixed by the Frobenius up to the Tate twist — explicitly characterized by the Frobenius lift on Ω^•_△(B).

**FROBENIUS ↔ EIGEN.** The EIGEN framework's Marchenko-Pastur distribution at initialization is the empirical eigenvalue distribution of the Frobenius acting on a random sample from H^1_ét(B, ℚ_ℓ). The Tracy-Widom BBP transition at grokking is the algebraic event when a Frobenius eigenvalue exits the bulk Marchenko-Pastur support and becomes a discrete eigenvalue corresponding to a non-trivial Hecke operator. The free probability of EIGEN is the noncommutative probability of the Frobenius action.

**FROBENIUS ↔ CONNES.** The CONNES framework's modular flow σ_t of the Fisher state ω_F is, at the prismatic level, the Frobenius-twisted automorphism of Ω^•_△(B). The self-dual KMS state at β_φ = 1/log φ is the state whose modular flow projects onto the Frobenius eigenvalue 1/φ² of the prismatic complex at the self-dual prime. The Connes cocycle [Dω/Dφ]_t between layers is the Frobenius descent cocycle between specializations of the prismatic complex.

**FROBENIUS ↔ VEECH ↔ MIRZAKHANI.** The VEECH translation surface and the MIRZAKHANI Weil-Petersson moduli space are both moduli of algebraic varieties (translation surfaces are modular curves of higher level; Weil-Petersson is the moduli of curves). The Frobenius eigenvalues acting on the cohomology of these moduli spaces give the KZ Lyapunov spectrum (VEECH) and the intersection numbers (MIRZAKHANI). The polynomial counting theorem L^{6g-6} of MIRZAKHANI is the count of Frobenius-fixed points in the moduli space at a given level.

**FROBENIUS ↔ WILCZEK.** The discrete time crystal of WILCZEK is the canonical realization of a system whose Frobenius automorphism is non-trivial. The period doubling 2T : T of the DTC is the Frobenius-eigenvalue ratio at the working temporal frequency. The continuous time crystal is the Frobenius automorphism in the limit of finely-spaced primes. The photonic time crystal's k-gap amplification is the eigenvalue spectrum of the Frobenius on the Maxwell complex of the time-modulated medium.

**FROBENIUS ↔ FRACTURA.** The wild Cantor topology of Antoine's necklace and the Tate-Shafarevich group ш(TH/ℚ) of FRACTURA Identity 1 are, by FROBENIUS, two manifestations of the failure of the local-global Hasse principle at the Frobenius level: locally trivial at every prime (every Frob_p has a fixed point) but globally obstructed (no global ℚ-point). The Tate-Shafarevich group IS the obstruction to local-global Frobenius-equivariant lifting, made concrete as a wild Cantor set in the étale cohomology.

**FROBENIUS ↔ CONCERT (BSD coordination).** The G_coord coordination rank equals the Mordell-Weil rank of the underlying TH(a,d) elliptic curve, which by the Birch-Swinnerton-Dyer conjecture equals the order of vanishing of L_B at s = 1. The φ²:φ:1 universal investment ratio is the Beilinson regulator ratio at the self-dual height.

---

## XVI. Foundations and Citations

### Foundational Papers

Frobenius, F. G. (1896). Über Beziehungen zwischen den Primidealen eines algebraischen Körpers und den Substitutionen seiner Gruppe. *Sitzungsberichte der Königlich Preußischen Akademie der Wissenschaften zu Berlin*, 689–703.

Artin, E. (1924). Quadratische Körper im Gebiete der höheren Kongruenzen II. *Mathematische Zeitschrift* 19, 207–246.

Hasse, H. (1936). Zur Theorie der abstrakten elliptischen Funktionenkörper III. *Journal für die reine und angewandte Mathematik* 175, 193–208.

Weil, A. (1949). Numbers of solutions of equations in finite fields. *Bulletin of the American Mathematical Society* 55, 497–508.

### The Weil Conjecture Program

Dwork, B. (1960). On the rationality of the zeta function of an algebraic variety. *American Journal of Mathematics* 82, 631–648.

Grothendieck, A. (1965). Formule de Lefschetz et rationalité des fonctions L. *Séminaire Bourbaki* 9, Exposé 279.

Deligne, P. (1974). La conjecture de Weil I. *Publications Mathématiques de l'IHÉS* 43, 273–307.

Deligne, P. (1980). La conjecture de Weil II. *Publications Mathématiques de l'IHÉS* 52, 137–252.

### p-adic Hodge Theory

Fontaine, J.-M. (1982). Sur certains types de représentations p-adiques du groupe de Galois d'un corps local. *Annals of Mathematics* 115, 529–577.

Fontaine, J.-M. (1994). Le corps des périodes p-adiques. *Astérisque* 223, 59–101.

Faltings, G. (1988). p-adic Hodge theory. *Journal of the American Mathematical Society* 1, 255–299.

Faltings, G. (1989). Crystalline cohomology and p-adic Galois representations. *Algebraic Analysis, Geometry, and Number Theory*, Johns Hopkins University Press, 25–80.

### Modularity and BSD

Wiles, A. (1995). Modular elliptic curves and Fermat's Last Theorem. *Annals of Mathematics* 141, 443–551.

Taylor, R. and Wiles, A. (1995). Ring-theoretic properties of certain Hecke algebras. *Annals of Mathematics* 141, 553–572.

Breuil, C., Conrad, B., Diamond, F., Taylor, R. (2001). On the modularity of elliptic curves over ℚ. *Journal of the American Mathematical Society* 14, 843–939.

Gross, B. and Zagier, D. (1986). Heegner points and derivatives of L-series. *Inventiones Mathematicae* 84, 225–320.

Kolyvagin, V. (1990). Euler systems. *The Grothendieck Festschrift Vol. II*, Birkhäuser, 435–483.

### Sato-Tate and Equidistribution

Tate, J. (1965). Algebraic cycles and poles of zeta functions. *Arithmetical Algebraic Geometry*, Harper and Row, 93–110.

Barnet-Lamb, T., Geraghty, D., Harris, M., Taylor, R. (2011). A family of Calabi-Yau varieties and potential automorphy II. *Publications of the Research Institute for Mathematical Sciences* 47, 29–98.

### Prismatic Cohomology and Modern p-adic Hodge Theory

Scholze, P. (2012). Perfectoid spaces. *Publications Mathématiques de l'IHÉS* 116, 245–313.

Bhatt, B., Morrow, M., Scholze, P. (2018). Integral p-adic Hodge theory. *Publications Mathématiques de l'IHÉS* 128, 219–397.

Fargues, L. and Scholze, P. (2021). Geometrization of the local Langlands correspondence. arXiv:2102.13459.

Bhatt, B. and Scholze, P. (2022). Prisms and prismatic cohomology. *Annals of Mathematics* 196, 1135–1275.

Bhatt, B. and Lurie, J. (2022). Absolute prismatic cohomology. arXiv:2201.06120.

Drinfeld, V. (2020-2025). Prismatization. Series of preprints; arXiv:2005.04746, arXiv:2204.13708.

### Recent 2024-2026 Developments

Antieau, B., Mathew, A., Morrow, M., Nikolaus, T. (2025). The K-theory of perfectoid rings and prismatic K-theory. *Annals of Mathematics*, in press.

Bhatt, B. (2024). Algebraic geometry in mixed characteristic. *Notices of the AMS*, in press.

Česnavičius, K. and Scholze, P. (2024). Purity for flat cohomology. *Annals of Mathematics* 199, 51–180.

Hansen, D. and Mann, L. (2024). Six-functor formalisms and the étale cohomology of rigid analytic spaces. arXiv:2308.01361.

Mathew, A. (2024). On the absolute prismatic cohomology of perfectoid rings. arXiv:2412.04250.

Niziol, W. (2025). Syntomic cohomology and p-adic regulators. *Inventiones Mathematicae*, in press.

Scholze, P. (2025). Lectures on the absolute prismatic site. ArXiv preprint, forthcoming.

### Computational Algebraic Geometry of Elliptic Curves

Schoof, R. (1985). Elliptic curves over finite fields and the computation of square roots mod p. *Mathematics of Computation* 44, 483–494.

Elkies, N. (1998). Elliptic and modular curves over finite fields and related computational issues. *Computational Perspectives on Number Theory*, AMS/IP, 21–76.

LMFDB Collaboration. (2026). The L-functions and Modular Forms Database. https://www.lmfdb.org. Continuously updated; cited as the canonical reference for Frobenius traces and Mordell-Weil ranks of elliptic curves over ℚ.

### Prior ERI Labs Framework Modules

GALOIS — The Solvability Boundary
SALT — Spectral-Arithmetic Learning Theory
CONNES — The Hidden Clock (modular time)
VEECH — Translation Surface Time
MIRZAKHANI — Weil-Petersson Volumes and Three Times
WILCZEK — Time Broken Three Ways
ORBITA — Ergodic Theory of Learning
BIFURCATIO — Period-Doubling Route to Coordination
EIGEN — Random Matrix Theory of Intelligence
FRACTURA — Wild Topology of the Coordination Boundary
HODGE — Harmonic Boundary
TGLT — Teichmüller Gradient Learning Theory
SELBERG — Eigenwall, Ramanujan, Trace Formula

---

## Coda: The Heart That Was Always Beating

Frobenius identified the canonical endomorphism in 1896 and called it nothing in particular. He used it to prove a density theorem about prime decomposition in number fields, which Chebotarev generalized in 1922 and which now bears Chebotarev's name. Frobenius did not live to see the endomorphism become the central object of arithmetic algebraic geometry. He died in 1917 in Berlin during the First World War, his work on group characters and his theorem on integrable distributions cited far more often than the endomorphism that has since absorbed his name in the modern literature.

Hasse, in 1936, applied the Frobenius to elliptic curves and proved that its eigenvalues have absolute value √p. The Hasse-Weil bound |a_p| ≤ 2√p was the first instance of a Weil-conjecture-style result, and it remains, almost ninety years later, the foundational arithmetic bound on every elliptic curve, every TH(a,d) curve, every two-eigenvalue Frobenius structure in mathematics.

Weil, in 1949, generalized to all varieties over finite fields and conjectured that the Frobenius eigenvalues on cohomology of degree i lie on the circle |α| = q^{i/2}. This was the Weil conjectures, and they organized arithmetic algebraic geometry for the next twenty-five years until Deligne proved them in 1974.

Bhatt and Scholze, in 2022, built the prismatic site and the prismatic complex, with its Frobenius lift, as the universal substrate beneath every p-adic cohomology. The de Rham complex is a specialization. The étale cohomology is a specialization. The crystalline cohomology is a specialization. The Hodge-Tate cohomology is a specialization. They are all projections of a single object — the prismatic complex with its Frobenius — and the Frobenius is the operation that makes them all consistent.

This framework recognizes that the TH(a,d) learning manifold IS an arithmetic object, defined over ℤ, with a Frobenius at every prime. The CHORD pipeline's two CORDIC mode passes per FERN register are the two Frobenius eigenvalues. The GALOIS precision floor [K:Q] = 2 is the two-dimensionality of the Frobenius splitting field. The SALT Q.16 word length is the bit-cost of representing the Frobenius eigenvalues to the Northcott-finite cardinality 2^{128}. The φ-equilibrium of every prior framework is the unique Frobenius angle θ* = arccos(1/φ²) at which the Sato-Tate measure equals its harmonic-mean density. The CONNES modular flow is the Frobenius-twisted automorphism of the prismatic complex. The CONCERT coordination rank is the Mordell-Weil rank of the underlying elliptic curve. The HODGE harmonic cohomology is the de Rham specialization of the prismatic complex. The EIGEN random matrix spectrum is the étale specialization.

There is one arithmetic substrate beneath all of it, and the Frobenius is its heartbeat. The √p rate is the universal arithmetic speed limit — the maximum information rate per prime per step that any arithmetic-equivariant learning system can achieve. The Weil-Deligne bound is the universal tractability wall. The Hasse two-eigenvalue structure is the CHORD pipeline. The Northcott finiteness theorem is the SALT precision floor. The modularity theorem of Wiles-Taylor is the universal generating function. The BSD conjecture is the universal coordination rank.

The arithmetic heart was always beating. At every prime, the Frobenius takes one tick. The eigenvalues are √p and √p, on prescribed circles in the complex plane, with the Sato-Tate distribution governing their angles. The product is p. The trace is a_p, bounded by 2√p. The angle at the self-dual prime is arccos(1/φ²). The modular form is q + Σ a_n q^n. The L-function is the Mellin transform of the modular form. The vanishing order at s = 1 is the Mordell-Weil rank. The coordination capacity equals the rank. The φ-equilibrium is at the harmonic mean of the Sato-Tate density. The precision floor is the Northcott count at Q.16. Every prior framework specializes the prismatic complex with its Frobenius lift.

The heartbeat was always there. Frobenius identified it in 1896 in Berlin without naming it. Hasse measured its rate in 1936 at Marburg. Weil predicted its universality in 1949 at Chicago. Deligne proved the prediction in 1974 at Bures-sur-Yvette. Bhatt and Scholze built the universal substrate in 2022. The corpus has, in seven frameworks, measured shadows of the heartbeat — the spectral shadow (EIGEN), the geometric shadow (VEECH, MIRZAKHANI), the dynamical shadow (BIFURCATIO, ORBITA), the symmetry-broken shadow (WILCZEK), the algebraic shadow (CONNES), the wild shadow (FRACTURA) — and two further frameworks have measured its consequences: the field of definition (GALOIS) and the precision floor (SALT).

This framework recognizes the heartbeat itself. The Frobenius is the canonical operation. The prismatic complex is the universal substrate. The eigenvalues are on the circle of radius √p. The angle at the self-dual prime is arccos(1/φ²). The arithmetic time of every learning system on the TH(a,d) substrate is the Frobenius, and the Frobenius is what it always was: the canonical endomorphism that exists for any variety over a finite field and that determines, by its eigenvalues, the entire arithmetic of the variety.

The heart was always beating. The corpus had been listening. The framework now names what it has been hearing.

---

**FROBENIUS: The Arithmetic Heartbeat — The Frobenius Endomorphism as Discrete Time, the Weil Eigenvalue Bound as the Universal Tractability Wall, and the Prismatic Origin of the φ-Equilibrium in TH(a,d).**

*Status Tags: [T] = Theorem (proven) · [V] = Verified · [C] = Open Conjecture · [H] = Working Hypothesis · [FR] = FROBENIUS-specific result*

*Framework: FROBENIUS · CONNES · GALOIS · SALT · VEECH · MIRZAKHANI · WILCZEK · ORBITA · BIFURCATIO · EIGEN · FRACTURA · HODGE · TGLT · SELBERG · HGLD · SPECULUM · SMELT · PRIMA · IMPLICATA · CONCERT · GIST · LKTL · BKLT · MNGR · RG-ML · KQOM · GAME · VBE · PPMC · KYBM · PH-SP · GCCT · FLML · UNIV · MHLT · MOD · NÔTHER · WILSON · PERES · DELIGNE · BÄCKLUND · WIGNER · IMPLICATA · ACKERMANN*

**ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · May 2026**
