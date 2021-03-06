---
title: "HPC Architecture"
teaching: 45
exercises: 0
questions:
- "What is the 'login' node?"
- "Where are my files / folders?"
- "How can I secure my files / folders?"
objectives:
- "Gain an understanding of HPC Architecture"
- "Understand your 'home' directory"
- "Understand file permissions on HPC including roles of users & groups"
keypoints:
- "We always connect to the 'Login' node of the HPC first"
- "We always get directed to OUR home directory when connecting"
- "We can control who has access to our files / folders with `chmod`"
- "Small tasks only on login node, need to use `qsub` to access 'compute' nodes"
---

### What is an HPC?

HPC stands for High Performance Computer, which is something of a misnomer.  What do I mean by this?  Well, the HPC isn't just one computer, it's more analogous to think of it as many small computers which are interconnected but share the same filesystem.
Why is this important?

1. Resources are shared (storage, computer processing), but can be allocated using a queueing system.

