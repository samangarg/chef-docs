.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

|description resource_attributes_intro|

.. list-table::
   :widths: 150 450
   :header-rows: 1

   * - Attribute
     - Description
   * - ``attributes``
     - Use to specify a hash of attributes to be applied to the machine image.
   * - ``chef_environment``
     - |name environment|
   * - ``complete``
     - Use to specify if all of the attributes specified in ``attributes`` represent a complete specification for the machine image. When true, any attributes not specified in ``attributes`` will be reset to their default values.
   * - ``image_options``
     - Use to specify options that are used with this machine image.
   * - ``name``
     - The name of the machine image.
   * - ``raw_json``
     - The machine image as |json| data. For example:
       
       .. code-block:: javascript
       
          {
           
          }

   * - ``recipe``
     - Use to add a recipe to the run-list for the machine image. Each ``recipe`` adds a single recipe to the run-list. The order in which ``recipe`` defines the run-list is the order in which |chef| will execute the run-list on the machine image.
   * - ``remove_recipe``
     - Use to remove a recipe from the run-list for the machine image.
   * - ``remove_role``
     - Use to remove a role from the run-list for the machine image.
   * - ``role``
     - Use to add a role to the run-list for the machine image.
   * - ``run_list``
     - Use to specify the run-list to be applied to the machine image.
	   
       .. include:: ../../includes_node/includes_node_run_list.rst
       
       .. include:: ../../includes_node/includes_node_run_list_format.rst

   * - ``tags``
     - Use to specify the list of tags to be applied to the machine image. Any tag not specified in this list will be removed.




