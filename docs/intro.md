# Introduction

`cloudor` is a cloud middleware service that faciliates running container jobs on a variety of cloud providers. The alpha release focuses on supporting CUDA-accelerated docker-based jobs, even though it can be used to run x64 container jobs.

## Why uses `cloudor`

You should consider using `cloudor` service if:

* Your application is CUDA-accelerated and preferably needs NVIDIA GPUs
* Your application is not very latency-sensitive and its typical runt time ranges from minutes to hours. (A typical HPC job)

User cases:

* Test on different generations of GPUs
* Reduce the workload in on-premise servers
* Stay neutral on cloud platforms, preventing vendor lock-in
* Deliver ready-to-run code to customers

## What applications are **NOT** suited for cloudor

* Latency-critical applications. Currently `cloudor` does not maintain a "persistent" server for each kind of instances. Therefore, the user may very likely need to wait for the boot time, which can take one to several minutes long.
* a continuous service (e.g. web server): cloudor is tailored for batch job that finishes within finite runtime.
