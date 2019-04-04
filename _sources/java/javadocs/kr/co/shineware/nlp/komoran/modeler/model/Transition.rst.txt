.. java:import:: java.util.zip GZIPInputStream

.. java:import:: java.util.zip GZIPOutputStream

.. java:import:: kr.co.shineware.nlp.komoran.interfaces FileAccessible

Transition
==========

.. java:package:: kr.co.shineware.nlp.komoran.modeler.model
   :noindex:

.. java:type:: public class Transition implements FileAccessible

Constructors
------------
Transition
^^^^^^^^^^

.. java:constructor:: public Transition()
   :outertype: Transition

Transition
^^^^^^^^^^

.. java:constructor:: public Transition(int size)
   :outertype: Transition

Methods
-------
get
^^^

.. java:method:: public Double get(int prevId, int curId)
   :outertype: Transition

load
^^^^

.. java:method:: @Override public void load(String filename)
   :outertype: Transition

load
^^^^

.. java:method:: public void load(File file)
   :outertype: Transition

load
^^^^

.. java:method:: public void load(InputStream inputStream)
   :outertype: Transition

put
^^^

.. java:method:: public void put(int prevId, int curId, double transitionScore)
   :outertype: Transition

save
^^^^

.. java:method:: @Override public void save(String filename)
   :outertype: Transition

