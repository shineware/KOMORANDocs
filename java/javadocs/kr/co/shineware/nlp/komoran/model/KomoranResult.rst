.. java:import:: kr.co.shineware.nlp.komoran.constant SYMBOL

.. java:import:: kr.co.shineware.nlp.komoran.core.model LatticeNode

.. java:import:: kr.co.shineware.nlp.komoran.parser KoreanUnitParser

.. java:import:: kr.co.shineware.util.common.model Pair

KomoranResult
=============

.. java:package:: kr.co.shineware.nlp.komoran.model
   :noindex:

.. java:type:: public class KomoranResult

Constructors
------------
KomoranResult
^^^^^^^^^^^^^

.. java:constructor:: public KomoranResult(List<LatticeNode> latticeNode, String jasoUnits)
   :outertype: KomoranResult

Methods
-------
getJasoUnits
^^^^^^^^^^^^

.. java:method:: public String getJasoUnits()
   :outertype: KomoranResult

getList
^^^^^^^

.. java:method:: public List<Pair<String, String>> getList()
   :outertype: KomoranResult

getMorphesByTags
^^^^^^^^^^^^^^^^

.. java:method:: public List<String> getMorphesByTags(String... str)
   :outertype: KomoranResult

getMorphesByTags
^^^^^^^^^^^^^^^^

.. java:method:: public List<String> getMorphesByTags(Collection<String> targetPosCollection)
   :outertype: KomoranResult

getNouns
^^^^^^^^

.. java:method:: public List<String> getNouns()
   :outertype: KomoranResult

getPlainText
^^^^^^^^^^^^

.. java:method:: public String getPlainText()
   :outertype: KomoranResult

getResultNodeList
^^^^^^^^^^^^^^^^^

.. java:method:: public List<LatticeNode> getResultNodeList()
   :outertype: KomoranResult

getTokenList
^^^^^^^^^^^^

.. java:method:: public List<Token> getTokenList()
   :outertype: KomoranResult

