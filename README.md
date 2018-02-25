# BaaS-recipes

The BPaaS recipe is a configuration part of the runtime of a workspace. Every stack is based on a BPaaS recipe and contains meta information that defines how the workspace runtime should be created. When creating custom workspace runtime it’s often best to create a custom stack with a custom recipe.

Workspaces can have a single runtime or multiple runtimes. For example to develop a DApp for ethereum using truffle framework you may need to have a stack containing:
 -your development machine with truffle and nodejs installed
 -a dedicated instance for ethereum test network
 -a geth node
 

Currently Morpheus BPaaS uses Docker containers to handle the runtimes, to create runtime(s) from Dockerfiles for a single-container runtime, or compose files to create single-container/multi-container runtime(s).

We are working to build some recipes for “Ready-to-go” stacks for blockchain developmet for ethereum , hyperledger and more. 
