📘 Practical 12 – Metropolis Algorithm & Deterministic Model
⭐ Aim

To implement the Metropolis Algorithm for sampling from a probability distribution and compare its results with a Deterministic Numerical Model for computing statistical quantities.

🧩 Part A – Metropolis Algorithm
🔹 What is the Metropolis Algorithm?

A Markov Chain Monte Carlo (MCMC) method used to generate samples from a target probability distribution when direct sampling is difficult. It constructs a Markov chain whose stationary distribution matches the target distribution.

🔹 Target Distribution

Standard Normal Distribution:
π(x) ∝ exp(−x² / 2)

🔹 Algorithm Steps

Start with an initial value x₀.

Propose x′ from a normal random walk: Normal(xₜ, proposal_std²).

Compute acceptance probability α = min(1, π(x′) / π(xₜ)).

Accept or reject using a uniform random number.

Repeat for many iterations, discard burn-in, and use remaining samples.

🔹 Summary

log_target_density(x) computes log π(x).

metropolis_sampler() runs the algorithm, returns samples & acceptance rate.

Histogram and sample statistics (mean ≈ 0, variance ≈ 1) verify correctness.

🔹 Observations

Sample distribution matches the true standard normal curve.

Acceptance rate depends on proposal_std.

Mean ≈ 0 and variance ≈ 1 confirm accurate sampling.

🧩 Part B – Deterministic Model
🔹 What is a Deterministic Model?

A method that produces the same output every time, without randomness. Here, numerical integration is used.

🔹 Approach Used

Grid-based numerical integration:

Create grid from −5 to 5.

Evaluate pdf values.

Normalize numerically.

Compute E[X²] ≈ Σ(x² · pdf(x) · dx).

🔹 Quantity Computed

Expected value E[X²] for N(0,1), theoretical value = 1.

🔄 Comparison
Method	Estimated E[X²]	Type
Metropolis Algorithm	~1.0006	Stochastic
Deterministic Model	~0.9999	Deterministic
True Value	1.0	Analytical

Both methods closely match the theoretical value.

📌 Advantages (Short)
Metropolis Algorithm

✔ Works for complex/high-dimensional distributions
✔ No need for normalized density
✘ Needs tuning & convergence checks
✘ Contains sampling noise

Deterministic Model

✔ Same output every run
✔ Very accurate in low dimensions
✘ Not practical for high dimensions
✘ Requires good grid selection

✅ Conclusion

Metropolis Algorithm successfully samples from a standard normal distribution.

Deterministic integration accurately computes E[X²].

Both methods give results close to the theoretical value, showing consistency between stochastic and deterministic approaches.
