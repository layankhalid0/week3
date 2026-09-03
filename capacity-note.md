# capacity-note

## Capacity note (team, one page)

### The numbers

Locked model: Qwen/Qwen2.5-1.5B-Instruct

Target p95 end-to-end latency (your SLO today): 3.0 seconds

Knee concurrency (highest concurrency whose p95 is still under target): 4

Tokens per second at the knee: 185.21

Max sustainable request rate at the target p95: 0.342 req/s

### The limiting family

Compute-bound: throughput continues increasing as concurrency rises, but p95 latency crosses the 3-second SLO at higher concurrency.

### Why the knee, not the peak

We report the knee because it is the highest concurrency that meets the latency SLO, while the peak throughput at higher concurrency violates the required response-time target.
