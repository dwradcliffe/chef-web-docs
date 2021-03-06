.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

The ``GET`` method is used to get a list of aliases for the specified organization.

This method has no parameters.

**Request**

.. code-block:: xml

   GET /organizations/NAME/aliases

**Response**

The response is similar to:

.. code-block:: javascript

   {
     "title": "array of aliases",
     "type": "array",
     "items": {
       "type": "object",
       "properties": {
         "id": {
           ...
         },
         "name": {
           ...
         },
         "org_name": {
           ...
         },
         "modified_by": {
           ...
         },
         "modified_at": {
           ...
         },
         "notification_type": {
           ...
         },
         "delivery_options": {
           ...
         }
       }
     },
     "definitions": {
       "hipchat": {
         ...
       },
       "http": {
         ...
       },
       "smtp": {
         ...
       }
     }
   }

**Response Codes**

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Response Code
     - Description
   * - ``200``
     - |response code 200 ok|
