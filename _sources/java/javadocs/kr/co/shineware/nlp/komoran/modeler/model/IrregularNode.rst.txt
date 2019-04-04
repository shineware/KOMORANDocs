.. java:import:: java.io Serializable

.. java:import:: java.util List

.. java:import:: kr.co.shineware.util.common.model Pair

IrregularNode
=============

.. java:package:: kr.co.shineware.nlp.komoran.modeler.model
   :noindex:

.. java:type:: public class IrregularNode implements Serializable

Methods
-------
equals
^^^^^^

.. java:method:: @Override public boolean equals(Object obj)
   :outertype: IrregularNode

getFirstPosId
^^^^^^^^^^^^^

.. java:method:: public int getFirstPosId()
   :outertype: IrregularNode

getInnerScore
^^^^^^^^^^^^^

.. java:method:: public double getInnerScore()
   :outertype: IrregularNode

getLastMorph
^^^^^^^^^^^^

.. java:method:: public String getLastMorph()
   :outertype: IrregularNode

getLastPosId
^^^^^^^^^^^^

.. java:method:: public int getLastPosId()
   :outertype: IrregularNode

getMorphFormat
^^^^^^^^^^^^^^

.. java:method:: public String getMorphFormat()
   :outertype: IrregularNode

getTokens
^^^^^^^^^

.. java:method:: public List<Pair<String, Integer>> getTokens()
   :outertype: IrregularNode

hashCode
^^^^^^^^

.. java:method:: @Override public int hashCode()
   :outertype: IrregularNode

setFirstPosId
^^^^^^^^^^^^^

.. java:method:: public void setFirstPosId(int firstPosId)
   :outertype: IrregularNode

setInnerScore
^^^^^^^^^^^^^

.. java:method:: public void setInnerScore(double innerScore)
   :outertype: IrregularNode

setLastMorph
^^^^^^^^^^^^

.. java:method:: public void setLastMorph(String lastMorph)
   :outertype: IrregularNode

setLastPosId
^^^^^^^^^^^^

.. java:method:: public void setLastPosId(int lastPosId)
   :outertype: IrregularNode

setMorphFormat
^^^^^^^^^^^^^^

.. java:method:: public void setMorphFormat(String morphFormat)
   :outertype: IrregularNode

setTokens
^^^^^^^^^

.. java:method:: public void setTokens(List<Pair<String, Integer>> irrNodeTokens)
   :outertype: IrregularNode

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: IrregularNode

