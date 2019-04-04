.. java:import:: java.io File

.. java:import:: java.io InputStream

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: kr.co.shineware.ds.aho_corasick AhoCorasickDictionary

.. java:import:: kr.co.shineware.nlp.komoran.interfaces FileAccessible

IrregularTrie
=============

.. java:package:: kr.co.shineware.nlp.komoran.modeler.model
   :noindex:

.. java:type:: public class IrregularTrie implements FileAccessible

Constructors
------------
IrregularTrie
^^^^^^^^^^^^^

.. java:constructor:: public IrregularTrie()
   :outertype: IrregularTrie

Methods
-------
getTrieDictionary
^^^^^^^^^^^^^^^^^

.. java:method:: public AhoCorasickDictionary<List<IrregularNode>> getTrieDictionary()
   :outertype: IrregularTrie

init
^^^^

.. java:method:: public void init()
   :outertype: IrregularTrie

load
^^^^

.. java:method:: @Override public void load(String filename)
   :outertype: IrregularTrie

load
^^^^

.. java:method:: public void load(File file)
   :outertype: IrregularTrie

load
^^^^

.. java:method:: public void load(InputStream inputStream)
   :outertype: IrregularTrie

put
^^^

.. java:method:: public void put(String irr, IrregularNode irrNode)
   :outertype: IrregularTrie

save
^^^^

.. java:method:: @Override public void save(String filename)
   :outertype: IrregularTrie

