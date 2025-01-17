=================
gpflow.posteriors
=================

.. THIS IS AN AUTOGENERATED RST FILE
.. GENERATED BY `generate_rst.py`
.. DATE: 29/04/21



gpflow.posteriors.AbstractPosterior
-----------------------------------

.. autoclass:: gpflow.posteriors.AbstractPosterior
   :show-inheritance:
   :members:


gpflow.posteriors.BasePosterior
-------------------------------

.. autoclass:: gpflow.posteriors.BasePosterior
   :show-inheritance:
   :members:


gpflow.posteriors.FallbackIndependentLatentPosterior
----------------------------------------------------

.. autoclass:: gpflow.posteriors.FallbackIndependentLatentPosterior
   :show-inheritance:
   :members:


gpflow.posteriors.FullyCorrelatedPosterior
------------------------------------------

.. autoclass:: gpflow.posteriors.FullyCorrelatedPosterior
   :show-inheritance:
   :members:


gpflow.posteriors.IndependentPosterior
--------------------------------------

.. autoclass:: gpflow.posteriors.IndependentPosterior
   :show-inheritance:
   :members:


gpflow.posteriors.IndependentPosteriorMultiOutput
-------------------------------------------------

.. autoclass:: gpflow.posteriors.IndependentPosteriorMultiOutput
   :show-inheritance:
   :members:


gpflow.posteriors.IndependentPosteriorSingleOutput
--------------------------------------------------

.. autoclass:: gpflow.posteriors.IndependentPosteriorSingleOutput
   :show-inheritance:
   :members:


gpflow.posteriors.LinearCoregionalizationPosterior
--------------------------------------------------

.. autoclass:: gpflow.posteriors.LinearCoregionalizationPosterior
   :show-inheritance:
   :members:


gpflow.posteriors.PrecomputeCacheType
-------------------------------------

.. autoclass:: gpflow.posteriors.PrecomputeCacheType
   :show-inheritance:
   :members:


gpflow.posteriors.create_posterior
----------------------------------

.. autofunction:: gpflow.posteriors.create_posterior


gpflow.posteriors.expand_independent_outputs
--------------------------------------------

.. autofunction:: gpflow.posteriors.expand_independent_outputs


gpflow.posteriors.fully_correlated_conditional
----------------------------------------------

.. autofunction:: gpflow.posteriors.fully_correlated_conditional


gpflow.posteriors.get_posterior_class
-------------------------------------

This function uses multiple dispatch, which will depend on the type of argument passed in:


.. code-block:: python

    gpflow.posteriors.get_posterior_class( Kernel, InducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_base_case(...)


.. autofunction:: gpflow.posteriors._get_posterior_base_case


.. code-block:: python

    gpflow.posteriors.get_posterior_class( MultioutputKernel, InducingPoints )
    # dispatch to -> gpflow.posteriors._get_posterior_fully_correlated_mo(...)


.. autofunction:: gpflow.posteriors._get_posterior_fully_correlated_mo


.. code-block:: python

    gpflow.posteriors.get_posterior_class( SharedIndependent, SeparateIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_independent_mo(...)


.. autofunction:: gpflow.posteriors._get_posterior_independent_mo


.. code-block:: python

    gpflow.posteriors.get_posterior_class( SeparateIndependent, SeparateIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_independent_mo(...)


.. autofunction:: gpflow.posteriors._get_posterior_independent_mo


.. code-block:: python

    gpflow.posteriors.get_posterior_class( SharedIndependent, SharedIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_independent_mo(...)


.. autofunction:: gpflow.posteriors._get_posterior_independent_mo


.. code-block:: python

    gpflow.posteriors.get_posterior_class( SeparateIndependent, SharedIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_independent_mo(...)


.. autofunction:: gpflow.posteriors._get_posterior_independent_mo


.. code-block:: python

    gpflow.posteriors.get_posterior_class( IndependentLatent, FallbackSeparateIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_independentlatent_mo_fallback(...)


.. autofunction:: gpflow.posteriors._get_posterior_independentlatent_mo_fallback


.. code-block:: python

    gpflow.posteriors.get_posterior_class( IndependentLatent, FallbackSharedIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_independentlatent_mo_fallback(...)


.. autofunction:: gpflow.posteriors._get_posterior_independentlatent_mo_fallback


.. code-block:: python

    gpflow.posteriors.get_posterior_class( LinearCoregionalization, SeparateIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_linearcoregionalization_mo_efficient(...)


.. autofunction:: gpflow.posteriors._get_posterior_linearcoregionalization_mo_efficient


.. code-block:: python

    gpflow.posteriors.get_posterior_class( LinearCoregionalization, SharedIndependentInducingVariables )
    # dispatch to -> gpflow.posteriors._get_posterior_linearcoregionalization_mo_efficient(...)


.. autofunction:: gpflow.posteriors._get_posterior_linearcoregionalization_mo_efficient



gpflow.posteriors.independent_interdomain_conditional
-----------------------------------------------------

.. autofunction:: gpflow.posteriors.independent_interdomain_conditional


gpflow.posteriors.mix_latent_gp
-------------------------------

.. autofunction:: gpflow.posteriors.mix_latent_gp


gpflow.posteriors.separate_independent_conditional_implementation
-----------------------------------------------------------------

.. autofunction:: gpflow.posteriors.separate_independent_conditional_implementation

