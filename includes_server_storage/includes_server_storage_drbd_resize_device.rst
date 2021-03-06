.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

After backing up the |chef server| data, make a note of the current size of the ``/dev/opscode/drbd`` logical volume and mountpoint. Run the following commands:

.. code-block:: bash

   sudo lvdisplay -v --units 4096k /dev/opscode/drbd

and then:

.. code-block:: bash

   df -k /var/opt/opscode/drbd/data

Verify that |drbd| is in good shape on both backend machines. Both the primary and secondary machines should show states similar to ``Primary/Secondary UpToDate/UpToDate``.

Run the following command:

.. code-block:: bash

   cat /proc/drbd

.. note:: Save these results to compare them to the same data post-resize.