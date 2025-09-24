#
 Cross–platform reuse of legacy microarrays with modern RNA–Seq is attractive but
 challenging: the same gene can follow different measurement distributions, and feature
 selection can leak label information and inflate performance. We develop SCOPES, a
 leak–free, multi–objective feature–selection framework that balances three goals: predictive
 accuracy (AUC), selection stability (Kuncheva), and cross–platform alignment (Maximum
 Mean Discrepancy, MMD). On matched TCGA–BRCA Agilent/RNA–Seq data, an initial
 label–informed F–score slab produced an apparently perfect microarray model (AUC≈1.0)
 but lost ∼ 0.30 AUC after transfer to RNA–Seq, revealing selection leakage and plat
form shift. Replacing the slab with an unsupervised MAD filter and enforcing patient–safe
 cross–validation exposed a clear trade–off on the Pareto front: an alignment–first solution
 with a single gene achieved modest source performance and slight transfer loss (AUCAgilent≈
 0.69, AUCRNA-Seq ≈ 0.61, ∆AUC ≈ −0.08), whereas a richer 30–gene signature reached
 near–perfect source AUC but transferred poorly (∆AUC≈−0.38) with higher MMD. These
 results show that more genes often buy source accuracy at the expense of portability.
 SCOPES makes this trade–off explicit and suggests selecting near a Pareto “knee” under
 explicit size and alignment constraints. Reporting both ∆AUC and an alignment metric
 provides a simple, reproducible framework for building cross–platform gene signatures.
#
