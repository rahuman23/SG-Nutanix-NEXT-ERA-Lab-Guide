.. title:: Welcome to Nutanix .NEXT on Tour Singapore Hands on Lab session

.. toctree::
  :maxdepth: 2
  :caption: Era
  :name: _era
  :hidden:

  era_deploy_and_register/era_deploy_and_register
  era_provision_postgresdb/era_provision_postgresdb
  era_clone_postgresdb/era_clone_postgresdb
  era_rest_api/era_rest_api

.. toctree::
  :maxdepth: 2
  :caption: Appendix
  :name: _appendix
  :hidden:

  appendix/glossary
  appendix/basics
  appendix/container_basics
  taskman/taskman
  tools_vms/linux_tools_vm_cloud-init
  tools_vms/windows_tools_vm


  .. _getting_started:

  ---------------
  Getting Started
  ---------------

  Welcome to Nutanix .NEXT on Tour Singapore Hands on Lab session! Each section has a lesson and an exercise to give you hands-on practice. The instructor explains the exercises and answers any additional questions that you may have.

  At the end of the bootcamp, attendees should understand the basic concepts and technologies that make up the Nutanix Enterprise Cloud stack and should be well prepared for a hosted or onsite proof-of-concept (POC) engagement.

  To access the cluster, enter the following URL - https://10.42.83.37:9440/console/#login in your browser.

  This will bring you the Prism Management interface.

  Networking
  ..........

  Hosted POC clusters follow a standard naming convention:

  - **Cluster Name** - PHX-POC083-ERA
  - **Subnet** - 110.42.83.0/25
  - **Cluster IP** - 10.42.83.37

  Secondary Network

  - **Secondary VLAN** - 831
  - **Secondary Subnet** - 255.255.255.128
  - **Secondary Gateway** - 10.42.83.129
  - **Secondary IP Range** - 10.42.83.132-254


  Credentials
  ...........

  .. note::

    The *<Cluster Password>* is unique to each cluster and will be provided by the leader of the Workshop.

  .. list-table::
     :widths: 25 35 40
     :header-rows: 1

     * - Credential
       - Username
       - Password
     * - Prism Element
       - admin
       - Nutanix.NEXT2019
     * - Prism Central
       - admin
       - Nutanix.NEXT2019
     * - Controller VM
       - nutanix
       - Nutanix.NEXT2019
     * - Prism Central VM
       - nutanix
       - Nutanix.NEXT2019

  Each cluster has a dedicated domain controller VM, **DC**, responsible for providing AD services for the **NTNXLAB.local** domain. The domain is populated with the following Users and Groups:

  .. list-table::
     :widths: 25 35 40
     :header-rows: 1

     * - Group
       - Username(s)
       - Password
     * - Administrators
       - Administrator
       - nutanix/4u
     * - SSP Admins
       - adminuser01-adminuser25
       - nutanix/4u
     * - SSP Developers
       - devuser01-devuser25
       - nutanix/4u
     * - SSP Power Users
       - poweruser01-poweruser25
       - nutanix/4u
     * - SSP Basic Users
       - basicuser01-basicuser25
       - nutanix/4u
