**************************
How To: Change Domain Name
**************************

#. Edit the **config.local.php** file in the root directory of your CS-Cart installation:

   .. list-table::
       :stub-columns: 1
       :widths: 10 30

       *   -   Before:
           -   .. code:: php

                   $config['http_host'] = 'old_domain';
                   $config['http_path'] = '';

                   $config['https_host'] = 'old_domain';
                   $config['https_path'] = '';

       *   -   After:
           -   .. code:: php

                   $config['http_host'] = 'new_domain';
                   $config['http_path'] = '';

                   $config['https_host'] = 'new_domain';
                   $config['https_path'] = '';

#. If you use CS-Cart (not Multi-Vendor):

   * Go to **Administration → Stores** in the admin panel of your CS-Cart installation.

   * Click on the name of the storefront to open its settings.

   * Change the domain there and save your changes.

     .. image:: img/storefront_domain.png
         :align: center
         :alt: Changing domain name in CS-Cart.

#. Delete or rename the */var/cache* directory to clear the cache of your store.
