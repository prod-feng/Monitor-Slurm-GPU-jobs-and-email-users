# Monitor-Slurm-GPU-jobs-and-email-users
monitor, slurm,gpu,email, performance

This is a lightweigted tool to monitot GPU HPC jobs, email users if their jobs under-utilizing the GPU resources.

Find under-performing GPU jobs, email users about it.

The plan is to set cron job to run it, like in a 10-minute interval. It will email users, if it finds that one job under-performs (like 20% average on multiple GPUs, or has 1+ idling GPUs) 3 times in a row.

Use "pdsh" to login to GPU nodes to get GPU usage information. So need a user account that can SSH login to nodes, like root, or other users who are allowed.

A quick and simple tool for this purpose.

