
# Theoretical Foundation

## Little's Law

Little's Law is a fundamental theorem in queuing theory, relating the average number of items in a queue (L), the average arrival rate of items (λ), and the average time an item spends in the system (W):

$` L = \lambda \times W `$

In the context of a computer system:
- $L$ represents the average number of concurrent tasks (threads).
- $` \lambda `$ denotes the arrival rate of requests.
- $W$ is the average response time.

## Poisson Distribution

The Poisson distribution describes the probability of a given number of events happening in a fixed interval of time, given a known average arrival rate. In performance testing, it models the rate at which requests are injected into the system by the load injector. If $\lambda$ is the average arrival rate, the probability of observing $k$ requests in a time period is given by:

$` P(X = k) = \frac{\lambda^k e^{-\lambda}}{k!} `$