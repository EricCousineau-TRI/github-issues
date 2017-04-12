Issue: GitHub-Flavored reStructuredText Ignores Image Dimensions
----

GitHub flavored rst does not appear to support image dimensions.

This following image should only be ``40px`` wide::

   .. image:: ./big_image.png
      :width: 40px

.. image:: ./big_image.png
   :width: 40px

As seen, it is not. If you inspect the HTML source, it only indicates ``max-width: 100%``.
