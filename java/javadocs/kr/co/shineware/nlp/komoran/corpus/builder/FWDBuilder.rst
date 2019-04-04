.. java:import:: java.io BufferedReader

.. java:import:: java.io BufferedWriter

.. java:import:: java.io FileReader

.. java:import:: java.io FileWriter

.. java:import:: java.util HashMap

.. java:import:: java.util List

.. java:import:: java.util Map

.. java:import:: java.util Set

.. java:import:: java.util Map.Entry

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser CorpusParser

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser.model ProblemAnswerPair

.. java:import:: kr.co.shineware.util.common.file FileUtil

FWDBuilder
==========

.. java:package:: kr.co.shineware.nlp.komoran.corpus.builder
   :noindex:

.. java:type:: public class FWDBuilder

Constructors
------------
FWDBuilder
^^^^^^^^^^

.. java:constructor:: public FWDBuilder()
   :outertype: FWDBuilder

Methods
-------
build
^^^^^

.. java:method:: public void build(String filename)
   :outertype: FWDBuilder

buildPath
^^^^^^^^^

.. java:method:: public void buildPath(String path, String suffix)
   :outertype: FWDBuilder

getThreshold
^^^^^^^^^^^^

.. java:method:: public int getThreshold()
   :outertype: FWDBuilder

save
^^^^

.. java:method:: public void save(String filename, int threshold)
   :outertype: FWDBuilder

setThreshold
^^^^^^^^^^^^

.. java:method:: public void setThreshold(int threshold)
   :outertype: FWDBuilder

