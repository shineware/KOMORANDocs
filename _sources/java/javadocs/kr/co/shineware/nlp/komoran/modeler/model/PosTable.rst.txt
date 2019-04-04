.. java:import:: java.nio.charset StandardCharsets

.. java:import:: java.util HashMap

.. java:import:: java.util Map

.. java:import:: java.util Map.Entry

.. java:import:: java.util Set

.. java:import:: kr.co.shineware.nlp.komoran.interfaces FileAccessible

PosTable
========

.. java:package:: kr.co.shineware.nlp.komoran.modeler.model
   :noindex:

.. java:type:: public class PosTable implements FileAccessible

Constructors
------------
PosTable
^^^^^^^^

.. java:constructor:: public PosTable()
   :outertype: PosTable

Methods
-------
getId
^^^^^

.. java:method:: public int getId(String pos)
   :outertype: PosTable

getPos
^^^^^^

.. java:method:: public String getPos(int id)
   :outertype: PosTable

load
^^^^

.. java:method:: @Override public void load(String filename)
   :outertype: PosTable

load
^^^^

.. java:method:: public void load(InputStream is)
   :outertype: PosTable

load
^^^^

.. java:method:: public void load(File file)
   :outertype: PosTable

put
^^^

.. java:method:: public void put(String pos)
   :outertype: PosTable

save
^^^^

.. java:method:: @Override public void save(String filename)
   :outertype: PosTable

size
^^^^

.. java:method:: public int size()
   :outertype: PosTable

