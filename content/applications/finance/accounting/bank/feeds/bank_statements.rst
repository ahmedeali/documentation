===============
Bank statements
===============

Importing bank statements allows keeping track of bank account transactions and reconcile them with
the ones recorded in Odoo.

With :doc:`the bank synchronization feature <bank_synchronization>` the process is going to be
automated. However, if you do not want to use it or if your bank is not yet supported, other
options exist:

- Import the bank statement files delivered by your bank;
- Register the bank statements manually.

Import bank statements files
============================

Odoo supports multiple file formats to import bank statements:

- SEPA recommended Cash Management format (CAMT.053);
- Comma-separated values (.CSV);
- Open Financial Exchange (.OFX);
- Quicken Interchange Format (.QIF);
- Belgium: Coded Statement of Account (.CODA).

To import a file, go to the Accounting dashboard and click on :guilabel:`Import (Statements)` in the
the :guilabel:`Bank` journal, or click on the drop-down menu (:guilabel:`⋮`) button and then on
:guilabel:`Import Statement`.

.. image:: bank_statements/bank-overview.png
   :align: center
   :alt: Import a bank statement file in Odoo Accounting

Next, select the file you want to import and click on :guilabel:`Upload`.

Once the file is uploaded, after setting the necessary formatting options and mapping the needed
columns, click on :guilabel:`import`. It is also possible to :guilabel:`test` the bank statement
file before importing it.

.. image:: bank_statements/import-bank-statement.png
   :align: center
   :alt: Register bank statements manually in Odoo Accounting

Register bank transactions manually
===================================

If needed, you can also record your bank transactions manually. To do so, go to the :guilabel:`Bank`
journal available in the :guilabel:`Accounting dashboard` and click on :guilabel:`Create`. Make sure
to fill out the :guilabel:`Partner` and :guilabel:`Label` field to ease the reconciliation process.

