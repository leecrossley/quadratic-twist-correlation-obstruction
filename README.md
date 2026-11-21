# A positive prime model that passes every fixed quadratic twist test

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24417499.svg)](https://doi.org/10.5281/zenodo.24417499)

This result is now maintained in [quadratic-mertens-first-crossings](https://github.com/leecrossley/quadratic-mertens-first-crossings/tree/main/results/quadratic-twist-correlation-obstruction). This repository is archived and keeps its releases and DOI.

The field of discriminant 13 exposed the earlier prime model because that model still copied its splitting pattern. This construction changes the signs on ordinary primes so that testing against 13 gives the prime sums of a nonprincipal character. The same assignment handles every other fixed quadratic reference.

At the start $`y=e^P/3`$, with $`D=13e^{2P}`$, the magnitude of the untwisted prime bias grows in proportion to $`\log D`$. Its decreasing Mertens average stays positive for every real start from 2 onwards in the central-zero case. At the same time, the normalised correlation with each fixed secondary character stays bounded from 2 through **any prescribed finite cutoff**, with the assignment chosen for that cutoff. With a close pair of zeros in place of the central zero, positivity can last through any prescribed power of $`D`$. The statement uses RH and quadratic Dirichlet GRH, which Alpöge's announced Dirichlet GRH theorem supplies. [Proof](PROOF.md) · [Announcement](https://alpo.ge/remark.pdf) · [Independent formal checks](https://math.mit.edu/~drew/grh/)

The continued products even have the degree-one zero counts with the expected change in the conductor term when twisting an odd discriminant whose only possible common prime factor with the reference conductor is 13. Adjusting when finitely many secondary coefficients begin leaves their zeros fixed. There is also a version where the added coefficients start immediately and each fixed secondary bias is $`O(\sqrt{\log D\,\log\log D})`$ through every fixed power of $`D`$. These are statements about a constructed prime assignment. The implication at a polynomial scale in genuine Yokoi fields remains open. [Comparison with earlier results](PRIOR-WORK.md)

To replay the finite prime construction and the arithmetic checks, install [requirements.txt](requirements.txt) and run

```sh
sh verify-release.sh
```

Two programs check the interpolated moments and period bounds on one finite instance, which illustrates the construction, and enclose $`L(1/2,\chi_{17})`$. The release includes the Lean source for five supporting lemmas. [Verification](CHECKS.md) · [File hashes](SHA256SUMS)
