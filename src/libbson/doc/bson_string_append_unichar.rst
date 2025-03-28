:man_page: bson_string_append_unichar

bson_string_append_unichar()
============================

.. warning::
   .. deprecated:: 1.29.0

Synopsis
--------

.. code-block:: c

  void
  bson_string_append_unichar (bson_string_t *string, bson_unichar_t unichar);

Parameters
----------

* ``string``: A :symbol:`bson_string_t`.
* ``unichar``: A :symbol:`bson_unichar_t`.

Description
-----------

Appends a unicode character to string. The character will be encoded into its multi-byte UTF-8 representation.

.. warning:: The length of the resulting string (including the ``NULL`` terminator) MUST NOT exceed ``UINT32_MAX``.
