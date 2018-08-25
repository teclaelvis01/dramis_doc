########
Modules
########

************************************************
Clinic Authorizations Monitoring Dashboard
************************************************

.. image:: _static/camd_dasboard.png

Requisitos iniciales
====================

Las autorizaciones que se deben ver en este dashboard son las siguientes:

* Autorizaciones activas que les quede menos de 8 unidades
* Autorizaciones activas que vencen en los próximos 15 días
* El “dashboard” debe estar dividido por especialidad OT, PT, ST
* La autorización en el “dashboard” debe tener un link que lleve directo a las autorizaciones del paciente
* Debe tener una columna donde se pueda poner la fecha en que se trabajó la autorización y autómaticamente deje de aparecer en el dashboard
* Las columnas que debe tener son las siguientes
* Debemos poder ver todas las transacciones por localidad de ser necesario (Davenport, St.Cloud)

Se presentan los archivos incolucrados en este dashboard.

FrontEnd
---------

  * ``/html/interface/wp_forms/index.php```
  * ``/html/interface/wp_forms/js/app.js```
  * ``/html/interface/wp_forms/js/view-components/camdComponent.js```
  * ``/html/interface/patient_file/summary/authorizations_full.php```
  * ``/html/interface/patient_file/summary/record_authorization.php```


Backend
---------
    * ``/html/api/index.php```
    * ``/html/api/controllers/WpFormController.php```
    * ``/html/api/modeles/Authorization.php```

.. note:: 
    Si se desea compilar los archivos del FrontEnd deberá ejecutarse el siguiente comando en la carpeta ``/html/interface/wp_forms/```

    .. code-block:: bash

        npm run build





************************************************
Clinic Subsequent Authorizations Management
************************************************

.. image:: _static/csam_dashboard.png

Requisitos iniciales
====================

* Este dashboard debe presentar todas las autorizaciones que no estén atadas a un referido y que tengan cualquier estatus menos activa e inactiva.
* La autorización en el “dashboard” debe tener un link que lleve directo a las autorizaciones del paciente
* El “dashboard” debe estar dividido por especialidad OT, PT, ST
* Las columnas que debe tener son las siguientes
* Debemos poder ver todas las transacciones por localidad de ser necesario (Davenport, St.Cloud)


Se presentan los archivos incolucrados en este dashboard.

FrontEnd
---------

  * ``/html/interface/wp_forms/index.php```
  * ``/html/interface/wp_forms/js/app.js```
  * ``/html/interface/wp_forms/js/view-components/csamdComponent.js```
  * ``/html/interface/patient_file/summary/authorizations_full.php```
  * ``/html/interface/patient_file/summary/record_authorization.php```


Backend
---------
    * ``/html/api/index.php```
    * ``/html/api/controllers/WpFormController.php```
    * ``/html/api/modeles/Authorization.php```

.. note:: 
    Si se desea compilar los archivos del FrontEnd deberá ejecutarse el siguiente comando en la carpeta ``/html/interface/wp_forms/```

    .. code-block:: bash

        npm run build




************************************************
CBHS Subsequent Authorizations Management
************************************************

.. image:: _static/cbhs_dashboard.png

Requisitos iniciales
====================

* Este dashboard debe presentar todas las autorizaciones que no estén atadas a un referido y que tengan cualquier estatus menos activa e inactiva
* La autorización en el “dashboard” debe tener un link que lleve directo a las autorizaciones del paciente
* El “dashboard” debe estar dividido por especialidad TCM, PSR, MHC
* Las columnas que debe tener son las siguientes
* Debemos poder ver todas las transacciones por localidad de ser necesario (Davenport, St.Cloud) (Es una columna adicional o un filtro )
* Poner como editable todas las columnas que se puedan editar y que los cambios puedan actualizar el récord del paciente.



Se presentan los archivos incolucrados en este dashboard.

FrontEnd
---------

  * ``/html/interface/wp_forms/index.php```
  * ``/html/interface/wp_forms/js/app.js```
  * ``/html/interface/wp_forms/js/view-components/cbhssamComponent.js```
  * ``/html/interface/patient_file/summary/authorizations_full.php```
  * ``/html/interface/patient_file/summary/record_authorization.php```


Backend
---------
    * ``/html/api/index.php```
    * ``/html/api/controllers/WpFormController.php```
    * ``/html/api/modeles/Authorization.php```

.. note:: 
    Si se desea compilar los archivos del FrontEnd deberá ejecutarse el siguiente comando en la carpeta ``/html/interface/wp_forms/```

    .. code-block:: bash

        npm run build



************************************************
CBHS Subsequent Authorizations Management (Corrigiendo funcionalidades)
************************************************

.. image:: _static/cbhssm.gif

Requisitos iniciales
====================

* Este dashboard debe presentar todas las autorizaciones que no estén atadas a un referido y que tengan cualquier estatus menos activa e inactiva
* La autorización en el “dashboard” debe tener un link que lleve directo a las autorizaciones del paciente
* El “dashboard” debe estar dividido por especialidad TCM, PSR, MHC
* Las columnas que debe tener son las siguientes
* Debemos poder ver todas las transacciones por localidad de ser necesario (Davenport, St.Cloud) (Es una columna adicional o un filtro )
* Poner como editable todas las columnas que se puedan editar y que los cambios puedan actualizar el récord del paciente.

Correciones
===========


* Columna de “auth requested date” no va en este dashboar
* Faltaron las siguientes columnas “units left, “end date” y “worked date”


Se presentan los archivos incolucrados en estla correción de este dashboard.

FrontEnd
---------

  * ``html/interface/wp_forms/assets/rev-manifest.json```
  * ``html/interface/wp_forms/index.php```
  * ``/html/interface/wp_forms/js/view-components/cbhssamComponent.js```



.. note:: 
    Si se desea compilar los archivos del FrontEnd deberá ejecutarse el siguiente comando en la carpeta ``/html/interface/wp_forms/```

    .. code-block:: bash

        npm run build
