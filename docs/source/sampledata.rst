Einfacher Einstieg
==========

Die Variable *bo* enthält das aktuelle Business Object. In einer mehrfach Auswahl von Datensätzen wird das komplette Script je markiertem Datensatz erneut ausgeführt. Um die Schleife muss sich also das Plugin in der einfachen Form nicht kümmern. 

Zeichenkette setzen
-------------------

.. code-block:: c#

  bo.Anzeigename = "Test";
  
In diesem Beispiel wird angenommen, das Business Object habe eine Eigenschaft *Anzeigename*, dessen Wert auf *Test* gesetzt wird. 
