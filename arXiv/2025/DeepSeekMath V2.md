This show how we can train model on the problems like proving which simple way of verification does not exists.

1. Train verifiers. We can train verifiers using correctness reward - but this cannot ensure that verifier points out real issue, not hallucinations. Thus this paper uses meta verifiers that verify the issues that verifiers found.
2. Train provers to do self verification using verification and meta verification rewards.
3. A kind of self-play between prover and verifier. But we need to make a label for new proofs. This is done by AI-assisted human-i