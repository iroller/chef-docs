.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

The following attributes can be used to define a guard that is evaluated during the execution phase of the |chef client| run:

.. list-table::
   :widths: 60 420
   :header-rows: 1

   * - Guard
     - Description
   * - ``not_if``
     - Use to prevent a resource from executing when the condition returns ``true``.
   * - ``only_if``
     - Use to allow a resource to execute only if the condition returns ``true``.

