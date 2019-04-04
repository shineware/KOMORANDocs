.. java:import:: kr.co.shineware.nlp.komoran.model MorphTag

LatticeNode
===========

.. java:package:: kr.co.shineware.nlp.komoran.core.model
   :noindex:

.. java:type:: public class LatticeNode

Constructors
------------
LatticeNode
^^^^^^^^^^^

.. java:constructor:: public LatticeNode()
   :outertype: LatticeNode

LatticeNode
^^^^^^^^^^^

.. java:constructor:: public LatticeNode(int beginIdx, int endIdx, MorphTag morphTag, double score)
   :outertype: LatticeNode

LatticeNode
^^^^^^^^^^^

.. java:constructor:: public LatticeNode(LatticeNode latticeNode)
   :outertype: LatticeNode

Methods
-------
getBeginIdx
^^^^^^^^^^^

.. java:method:: public int getBeginIdx()
   :outertype: LatticeNode

getEndIdx
^^^^^^^^^

.. java:method:: public int getEndIdx()
   :outertype: LatticeNode

getMorphTag
^^^^^^^^^^^

.. java:method:: public MorphTag getMorphTag()
   :outertype: LatticeNode

getPrevNodeIdx
^^^^^^^^^^^^^^

.. java:method:: public int getPrevNodeIdx()
   :outertype: LatticeNode

getScore
^^^^^^^^

.. java:method:: public double getScore()
   :outertype: LatticeNode

getTag
^^^^^^

.. java:method:: public String getTag()
   :outertype: LatticeNode

setBeginIdx
^^^^^^^^^^^

.. java:method:: public void setBeginIdx(int beginIdx)
   :outertype: LatticeNode

setEndIdx
^^^^^^^^^

.. java:method:: public void setEndIdx(int endIdx)
   :outertype: LatticeNode

setMorphTag
^^^^^^^^^^^

.. java:method:: public void setMorphTag(MorphTag morphTag)
   :outertype: LatticeNode

setPrevNodeIdx
^^^^^^^^^^^^^^

.. java:method:: public void setPrevNodeIdx(int prevNodeIdx)
   :outertype: LatticeNode

setScore
^^^^^^^^

.. java:method:: public void setScore(double score)
   :outertype: LatticeNode

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: LatticeNode

