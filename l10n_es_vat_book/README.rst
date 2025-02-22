============
Libro de IVA
============

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:e544dc97fc2cc7673c532080d5a242686cc3634db0fbcb87aa6e09ac3d06aa56
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fl10n--spain-lightgray.png?logo=github
    :target: https://github.com/OCA/l10n-spain/tree/17.0/l10n_es_vat_book
    :alt: OCA/l10n-spain
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/l10n-spain-17-0/l10n-spain-17-0-l10n_es_vat_book
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/l10n-spain&target_branch=17.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

Módulo que calcula el libro de IVA español.

Esto módulo introduce el menú "Libro de IVA" en Contabilidad -> Informe
-> Declaraciones AEAT -> Libro de IVA.

Es posible visualizar e imprimir por separado:

- Libro Registro de Facturas Emitidas
- Libro Registro de Facturas Recibidas

Es posible exportar los registros a archivo con extensión xlsx.

En el modo de visualización de los informes es posible navegar a los
asientos contables relacionados con la factura.

**Table of contents**

.. contents::
   :local:

Installation
============

Para instalar este modulo necesitas:

- account
- base_vat
- l10n_es
- l10n_es_aeat
- report_xlsx

Se instalan automáticamente si están disponibles en la lista de addons.

Consideraciones adicionales:

- Es importante que en facturas que deban aparecer en los libros
  registros, no sujetos a IVA, informar el tipo de IVA 'No Sujeto' en
  facturas. Para evitar que los usuarios olviden informarlo es
  recomendable instalar el módulo 'account_invoice_tax_required'.

Configuration
=============

Los códigos de impuestos incluidos en el Libro de IVA pueden verse en:
Contabilidad -> Configuración -> AEAT -> Mapeo AEAT libro de IVA

Los clientes utilizados para ventas por caja deben tener marcado el
campo "AEAT - Cliente anónimo" para que no se muestren advertencias por
no tener NIF informado siguiendo lo especificado en el formato BOE.

Usage
=====

1. Ve a *Contabilidad > Declaraciones AEAT > Libro de IVA*.
2. Crea un nuevo registro.
3. Escoge el periodo de tiempo para el libro.
4. Pulsa en "Calcular".
5. Escoge la opción de visualización o impresión preferida.

Known issues / Roadmap
======================

Funcionalidades del Libro Registro de IVA no incluídas por el momento:

- Criterio de caja
- Regímenes especiales de seguros, de agencias de viaje o de bienes
  usados.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/l10n-spain/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/l10n-spain/issues/new?body=module:%20l10n_es_vat_book%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
-------

* PRAXYA
* ForgeFlow
* Tecnativa

Contributors
------------

- Daniel Rodriguez <drl.9319@gmail.com>
- Jordi Ballester (ForgeFlow) <jordi.ballester@forgeflow.com>
- Luis M. Ontalba <luismaront@gmail.com>
- `Tecnativa <https://www.tecnativa.com/>`__:

  - Pedro M. Baeza
  - Carlos Dauden
  - Ernesto Tejeda

- Omar Castiñeira <omar@comunitea.com>
- Fernando La Chica <fernandolachica@gmail.com>
- Victor Garcia <victor.garcia@kayuulab.com>
- Luis Lafaurie <ldlafaurie@gmail.com>
- Eduardo de miguel <edu@moduon.team>

Maintainers
-----------

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/l10n-spain <https://github.com/OCA/l10n-spain/tree/17.0/l10n_es_vat_book>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
