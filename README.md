
# uc3-ai-scheduler

A small scheduler project for the UC3 AI experiments. This repository contains configuration examples and utilities to run scheduling tasks for experiments.

## Description

Structure of the Use Case: we have the Simulation env pod, that shouldn't be taken into account by the scheduler (it is just a proxy for reality).
Then we have the UC software node (from 1 to 6). These are the pods that should be scheduled on the computing continuum. In particular, Node 6 should always run on the edge, while Node 5 should be run on edge or not depending on the scheduler policy (e.g., we want to save enrgy on the edge, so we will schedule the pod on another hardware node).

- uc3-v11.yaml: configuration with pods on fixed hardware nodes.
- uc3-v12.yaml: configuration with pods on free hardware nodes.

