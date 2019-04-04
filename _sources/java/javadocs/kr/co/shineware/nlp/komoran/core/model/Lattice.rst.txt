.. java:import:: kr.co.shineware.ds.aho_corasick FindContext

.. java:import:: kr.co.shineware.nlp.komoran.constant SYMBOL

.. java:import:: kr.co.shineware.nlp.komoran.model MorphTag

.. java:import:: kr.co.shineware.nlp.komoran.model ScoredTag

.. java:import:: kr.co.shineware.util.common.model Pair

.. java:import:: java.util ArrayList

.. java:import:: java.util HashMap

.. java:import:: java.util List

.. java:import:: java.util Map

Lattice
=======

.. java:package:: kr.co.shineware.nlp.komoran.core.model
   :noindex:

.. java:type:: public class Lattice

Constructors
------------
Lattice
^^^^^^^

.. java:constructor:: public Lattice(Resources resource, Observation userDic)
   :outertype: Lattice

Lattice
^^^^^^^

.. java:constructor:: public Lattice(Resources resource, Observation userDic, int nbest)
   :outertype: Lattice

Methods
-------
appendEndNode
^^^^^^^^^^^^^

.. java:method:: public boolean appendEndNode()
   :outertype: Lattice

appendNode
^^^^^^^^^^

.. java:method:: public int appendNode(LatticeNode latticeNode)
   :outertype: Lattice

findNBestPath
^^^^^^^^^^^^^

.. java:method:: public List<List<LatticeNode>> findNBestPath()
   :outertype: Lattice

findPath
^^^^^^^^

.. java:method:: public List<LatticeNode> findPath()
   :outertype: Lattice

getLastIdx
^^^^^^^^^^

.. java:method:: public int getLastIdx()
   :outertype: Lattice

getNodeList
^^^^^^^^^^^

.. java:method:: public List<LatticeNode> getNodeList(int index)
   :outertype: Lattice

getPosTable
^^^^^^^^^^^

.. java:method:: public PosTable getPosTable()
   :outertype: Lattice

makeNode
^^^^^^^^

.. java:method:: public LatticeNode makeNode(int beginIdx, int endIdx, String morph, String tag, int tagId, double score, int prevNodeHash)
   :outertype: Lattice

printLattice
^^^^^^^^^^^^

.. java:method:: public void printLattice()
   :outertype: Lattice

put
^^^

.. java:method:: public void put(int beginIdx, int endIdx, List<Pair<String, String>> fwdResultList)
   :outertype: Lattice

put
^^^

.. java:method:: public void put(int beginIdx, int endIdx, IrregularNode irregularNode)
   :outertype: Lattice

put
^^^

.. java:method:: public boolean put(int beginIdx, int endIdx, String morph, String tag, int tagId, double score)
   :outertype: Lattice

retrievalIrregularNodes
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public Map<String, List<IrregularNode>> retrievalIrregularNodes(char jaso)
   :outertype: Lattice

retrievalObservation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public Map<String, List<ScoredTag>> retrievalObservation(char jaso)
   :outertype: Lattice

retrievalUserDicObservation
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public Map<String, List<ScoredTag>> retrievalUserDicObservation(char jaso)
   :outertype: Lattice

setLastIdx
^^^^^^^^^^

.. java:method:: public void setLastIdx(int lastIdx)
   :outertype: Lattice

setObservation
^^^^^^^^^^^^^^

.. java:method:: public void setObservation(Observation observation)
   :outertype: Lattice

setPosTable
^^^^^^^^^^^

.. java:method:: public void setPosTable(PosTable posTable)
   :outertype: Lattice

setTransition
^^^^^^^^^^^^^

.. java:method:: public void setTransition(Transition transition)
   :outertype: Lattice

