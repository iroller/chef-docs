.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

Using the |resource dsc_resource| has the following requirements:

* |windows management_framework| 5.0 February Preview (or higher), which includes |windows powershell| 5.0.10018.0
* The ``RefreshMode`` configuration setting in the Local Configuration Manager must be set to ``Disabled``
* The |resource dsc_script| resource  may not be used in the same run-list with the |resource dsc_resource|. This is because the |resource dsc_script| resource requires that ``RefreshMode`` in the Local Configuration Manager be set to ``Push``, whereas the |resource dsc_resource| resource requires it to be set to ``Disabled``
