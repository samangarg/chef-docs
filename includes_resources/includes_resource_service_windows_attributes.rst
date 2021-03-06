.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

|description resource_attributes_intro|

.. list-table::
   :widths: 150 450
   :header-rows: 1

   * - Attribute
     - Description
   * - ``init_command``
     - |command service_init| This is typically ``/etc/init.d/SERVICE_NAME``. The ``init_command`` attribute can be used to prevent the need to specify  overrides for the ``start_command``, ``stop_command``, and ``restart_command`` attributes. Default value: ``nil``.
   * - ``pattern``
     - |pattern process_table| Default value: ``service_name``.
   * - ``provider``
     - Optional. |provider resource_parameter| |see providers|
   * - ``reload_command``
     - |command service_reload|
   * - ``restart_command``
     - |command service_restart|
   * - ``run_as_password``
     - |password windows_service_run_as|
   * - ``run_as_user``
     - |user windows_service_run_as|
   * - ``service_name``
     - |name service| Default value: the ``name`` of the resource block. |see syntax|
   * - ``start_command``
     - |command service_start|
   * - ``startup_type``
     - Use to specify the startup type for a |windows| service. Possible values: ``:automatic``, ``:disabled``, or ``:manual``. Default value: ``:automatic``.
   * - ``status_command``
     - |command service_status|
   * - ``stop_command``
     - |command service_stop|
   * - ``supports``
     - |supports service| Default value: ``{ :restart => false, :reload => false, :status => false }`` for all platforms (except for the |redhat| platform family, which defaults to ``{ :restart => false, :reload => false, :status => true }``.)
   * - ``timeout``
     - |timeout|