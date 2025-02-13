# Elmer – understand complex physical processes in the natural world (training)

# About
This page documents the most important information, links and directory locations used in the hands-on demostration of Elmer code running on Setonix CPU and GPU.

# Elmer Overview
Elmer is an open-source multiphysical simulation software mainly developed by CSC – IT Center for Science (CSC). Elmer’s development started as a national collaboration with Finnish Universities, research institutes, and industry. After it’s open source publication, the use and development of Elmer have become largely international.
Elmer is a scientific software tool that helps researchers simulate and understand complex physical processes in the natural world. Think of it as a sophisticated digital laboratory where scientists can model everything from glacier movements and groundwater flow to heat transfer in the Earth’s systems. What makes Elmer particularly valuable is its ability to combine different types of physics—like how water flows, how materials deform, and how heat moves—all in one simulation. This is especially useful for climate scientists who need to understand how multiple environmental factors interact with each other. Plus, being open-source means it’s freely available to researchers worldwide, and it can run on supercomputers like Pawsey’s Setonix to tackle big scientific challenges.

## Access to Setonix
All participants of the course will obtain training account and password. We recommend to use training accounts during the session, this will allow us to utilise resources dedicated and reserved for the course. To login to Setonix, open your favourite Terminal and type:

    ssh couXXX@setonix.pawsey.org.au

## Submitting your first job on Setonix

## Submitting Elmer job on Setonix
Training materials are available on Setonix: `/scratch/courses01/elmer_parallel_demo.tar.gz`
Create your own copy of materials by:

    cd $MYSCRATCH
    cp /scratch/courses01/elmer_parallel_demo.tar.gz .
    tar zxf elmer_parallel_demo.tar.gz
    cd elmer_parallel_demo/

Content of the directory:

    $ ls
    elmer_flow_gcr.sif  elmer_flow.msh       linsys_rocm.sif      runelmer_gpu_serial.sh
    elmer_flow.geo      elmer_flow_rocm.sif  runelmer_cpu_mpi.sh  runpost.sh

* `runelmer_cpu_mpi.sh` - can be used to submit parallel MPI Elmer job on Setonix CPUs
* `runelmer_gpu_serial.sh` - can be used to submit single-GPU Elmer job on Setonix GPU
* `runpost.sh` - can be used to visualise results with Paraview; should be run on Setonix visualisation nodes (remote visualisation service - see below)

## Visualising your results
Documentation on how to use Paraview at Pawsey's remote visualisation service: 
* [Setonix Remote Visualisation Documentation](https://pawsey.atlassian.net/wiki/spaces/US/pages/51925070/Setonix+Remote+Visualisation)
* [Getting Started with Setonix Remote Visualisation](https://pawsey.atlassian.net/wiki/spaces/US/pages/51925068/Getting+Started+With+Setonix+Remote+Visualisation)
* [ParaView on Setonix Remote Visualisation](https://pawsey.atlassian.net/wiki/spaces/US/pages/51925146/ParaView+on+Setonix+Remote+Visualisation)
