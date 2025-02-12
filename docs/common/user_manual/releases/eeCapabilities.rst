.. _lbl-capabilities_eeuq:
.. role:: blue

************
Capabilities
************

**Version 3.3** of |app| was released **March 23**. The following lists the functionality available in this current version. (Note: New features and fixes in this release are marked :blue:`blue` in the following list of features.)


Structural Information Model
============================

Applications used to specify/select the structural model to be used in analysis.

#. MDOF: creating idealized multi-degree-of-freedom models
#. OpenSees: user-defined OpenSees models
#. Steel Building Model: automating steel frame design and modeling
#. Concrete Building Model: automating concrete moment frame design and modeling
#. MDOF-LU: MDOF shear building model
#. :blue:`SurrogateGP: surrogate model trained in EE-UQ`
#. :blue:`Multimodel: selecting multiple structural information models`

    
Earthquake Motion Event
=======================

Applications used to specify/select ground motions for the structure.

#.  Stochastic Ground Motion: simulating stochastic ground motion recordings
#.  PEER NGA Records: selecting and scaling PEER NGA West2 ground motions :blue:`[<- New option to select a suit of ground motions with uniformly populated IMs. This can be useful when training a surrogate model]`
#.  Site Response: propagating rock motions to the surface
#.  Multiple PEER: using multiple PEER recordings
#.  Multiple SimCenter: using multiple SimCenter-format recordings
#.  User Specified Database: selecting and scaling ground motions from the user-specified flatfile


Engineering Demand Parameter Generator
======================================

Applications to identify the output parameters of interest given the ground motion and structural model.

#. Standard Earthquake: maximum story drift ratio, lateral story displacement, peak floor acceleration
#. User Defined: user-specified EDP
#. :blue:`None: used only for surrogate model-based predictions`
    
    
Finite Element Application
==========================

Applications used to determine the response output parameters given the ground motion and structural model.

#.  OpenSees: Open System for Earthquake Engineering Simulation
#.  :blue:`CustomPy-Simulation: user-provided python script`
#.  :blue:`None: used only for surrogate model-based predictions`
#.  :blue:`Multimodel: selecting multiple finite element applications`

Uncertainty Quantification
==========================

Applications to perform the uncertainty quantification for the response parameters given the inputs and the random variables present.

#. Forward Uncertainty Propagation

     A. Dakota Options

        #. Monte Carlo Sampling (MCS)
        #. Latin Hypercube Sampling (LHS)
        #. Gaussian Process Regression
        #. Polynomial Chaos Expansion

     B. SimCenterUQ Options

        #. Monte Carlo Sampling (MCS)

           a. Resample from existing correlated dataset of samples

#. Global Sensitivity Analysis

     A. Dakota Sensitivity Options

        #. MCS
        #. LHS

     B. SimCenterUQ Sensitivity Options

        #. Probability Model-based Global Sensitivity Analysis (PM-GSA)

           a. Import input/output samples from data files


#. Surrogate Modeling

     A. SimCenterUQ Engine Surrogate Options:

        #. Probabilistic Learning on Manifolds (PLoM) Surrogate modeling
        #. :blue:`Gaussian Process Surrogate Modeling`
	   
