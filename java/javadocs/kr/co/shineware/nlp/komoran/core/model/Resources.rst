.. java:import:: java.io File

.. java:import:: java.io InputStream

.. java:import:: kr.co.shineware.nlp.komoran.constant FILENAME

.. java:import:: kr.co.shineware.nlp.komoran.modeler.model IrregularTrie

.. java:import:: kr.co.shineware.nlp.komoran.modeler.model Observation

.. java:import:: kr.co.shineware.nlp.komoran.modeler.model PosTable

.. java:import:: kr.co.shineware.nlp.komoran.modeler.model Transition

Resources
=========

.. java:package:: kr.co.shineware.nlp.komoran.core.model
   :noindex:

.. java:type:: public class Resources

Methods
-------
getIrrTrie
^^^^^^^^^^

.. java:method:: public IrregularTrie getIrrTrie()
   :outertype: Resources

getObservation
^^^^^^^^^^^^^^

.. java:method:: public Observation getObservation()
   :outertype: Resources

getTable
^^^^^^^^

.. java:method:: public PosTable getTable()
   :outertype: Resources

getTransition
^^^^^^^^^^^^^

.. java:method:: public Transition getTransition()
   :outertype: Resources

init
^^^^

.. java:method:: public void init()
   :outertype: Resources

load
^^^^

.. java:method:: public void load(String path)
   :outertype: Resources

loadIrregular
^^^^^^^^^^^^^

.. java:method:: public void loadIrregular(File file)
   :outertype: Resources

loadIrregular
^^^^^^^^^^^^^

.. java:method:: public void loadIrregular(InputStream inputStream)
   :outertype: Resources

loadObservation
^^^^^^^^^^^^^^^

.. java:method:: public void loadObservation(File file)
   :outertype: Resources

loadObservation
^^^^^^^^^^^^^^^

.. java:method:: public void loadObservation(InputStream inputStream)
   :outertype: Resources

loadPosTable
^^^^^^^^^^^^

.. java:method:: public void loadPosTable(File file)
   :outertype: Resources

loadPosTable
^^^^^^^^^^^^

.. java:method:: public void loadPosTable(InputStream file)
   :outertype: Resources

loadTransition
^^^^^^^^^^^^^^

.. java:method:: public void loadTransition(File file)
   :outertype: Resources

loadTransition
^^^^^^^^^^^^^^

.. java:method:: public void loadTransition(InputStream inputStream)
   :outertype: Resources

setIrrTrie
^^^^^^^^^^

.. java:method:: public void setIrrTrie(IrregularTrie irrTrie)
   :outertype: Resources

setObservation
^^^^^^^^^^^^^^

.. java:method:: public void setObservation(Observation observation)
   :outertype: Resources

setTable
^^^^^^^^

.. java:method:: public void setTable(PosTable table)
   :outertype: Resources

setTransition
^^^^^^^^^^^^^

.. java:method:: public void setTransition(Transition transition)
   :outertype: Resources

