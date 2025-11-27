This shows how we can train a model on problems like proving for which a simple verification method does not exist. Meta-verification is the central idea of this.

1. Train verifiers. We can train verifiers using correctness rewards - but this cannot ensure that the verifier points out a real issue, not hallucinations. Thus this paper uses meta verifiers that verify the issues that verifiers found.
2. Train provers to do self-verification using verification and meta-verification rewards.
3. A kind of self-play between prover and verifier. But we need to create labels for new proofs. This is done by AI-assisted manual annotation. First verification is done N times, and for issues found in verification, meta-verification is done M times. If they find k legitimate issues then it is incorrect. If no issues are found it is considered correct. A relaxed pessimistic scoring.
