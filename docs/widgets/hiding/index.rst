.. _hiding_widgets:

Hiding widgets
====================

Actually every widget can be hidden including texts, buttons, groups and so on.
It is managed by ``when`` attribute. It can be either a data key, a predicate function or a F-filter (from ``magic-filter``).

F-filter receives the data from the getter and other dialog data. You can refer to it, for example ``F["extended"]`` or ``F["dialog_data"]["user"]["name"]``

.. literalinclude:: ./example.py

.. image::  /resources/whenable.png

If you only change data setting ``"extended": True`` the window will look differently


.. image::  /resources/whenable_extended.png

.. autoclass:: aiogram_dialog.widgets.common.when.Predicate
   :special-members: __call__
