Zuweisen von Eigenschaften
==========

Die Variable *bo* enthält das aktuelle Business Object. In einer mehrfach Auswahl von Datensätzen wird das komplette Script je markiertem Datensatz erneut ausgeführt. Um die Schleife muss sich also das Plugin in der einfachen Form nicht kümmern. 

Zeichenkette
-------------------

.. code-block:: c#

  bo.Anzeigename = "Test";
  
In diesem Beispiel wird angenommen, das Business Object habe eine Eigenschaft *Anzeigename*, dessen Wert auf *Test* gesetzt wird. 

.. code-block:: c#

  bo.Anzeigename += "Test";
  
Durch den *+=* Operator wird der bisherigen Eigenschaft das Wort *Test* angehangen. 


Datum
-------------------

.. code-block:: c#

  bo.Datum = new DateTime(2017, 12, 24); // festes Datum unabhängig von vorher
  bo.Datum = bo.Datum.AddDays(5); // 5 Tage mehr als bisher
  bo.Datum = bo.Datum.AddMonths(-2); // 2 Monate weniger als bisher

Weitere Infos zu DateTime-Methoden in der `Microsoft MSDN <https://msdn.microsoft.com/de-de/library/system.datetime_methods(v=vs.110).aspx>`_
