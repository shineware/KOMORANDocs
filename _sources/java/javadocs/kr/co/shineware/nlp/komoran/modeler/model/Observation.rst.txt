.. java:import:: java.io File

.. java:import:: java.io InputStream

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: kr.co.shineware.ds.aho_corasick AhoCorasickDictionary

.. java:import:: kr.co.shineware.nlp.komoran.interfaces FileAccessible

.. java:import:: kr.co.shineware.nlp.komoran.interfaces UnitParser

.. java:import:: kr.co.shineware.nlp.komoran.model ScoredTag

.. java:import:: kr.co.shineware.nlp.komoran.parser KoreanUnitParser

Observation
===========

.. java:package:: kr.co.shineware.nlp.komoran.modeler.model
   :noindex:

.. java:type:: public class Observation implements FileAccessible

Constructors
------------
Observation
^^^^^^^^^^^

.. java:constructor:: public Observation()
   :outertype: Observation

Methods
-------
getTrieDictionary
^^^^^^^^^^^^^^^^^

.. java:method:: public AhoCorasickDictionary<List<ScoredTag>> getTrieDictionary()
   :outertype: Observation

load
^^^^

.. java:method:: @Override public void load(String filename)
   :outertype: Observation

load
^^^^

.. java:method:: public void load(File file)
   :outertype: Observation

load
^^^^

.. java:method:: public void load(InputStream is)
   :outertype: Observation

put
^^^

.. java:method:: public void put(String word, String tag, int tagId, double observationScore)
   :outertype: Observation

save
^^^^

.. java:method:: @Override public void save(String filename)
   :outertype: Observation

