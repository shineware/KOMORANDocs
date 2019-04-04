.. java:import:: kr.co.shineware.ds.aho_corasick FindContext

.. java:import:: kr.co.shineware.nlp.komoran.modeler.model IrregularNode

.. java:import:: java.util List

.. java:import:: java.util Map

.. java:import:: java.util Set

IrregularParser
===============

.. java:package:: kr.co.shineware.nlp.komoran.core.model
   :noindex:

.. java:type:: public class IrregularParser implements Parser

Constructors
------------
IrregularParser
^^^^^^^^^^^^^^^

.. java:constructor:: public IrregularParser(Resources resources)
   :outertype: IrregularParser

Methods
-------
parse
^^^^^

.. java:method:: @Override public void parse()
   :outertype: IrregularParser

setParseInfo
^^^^^^^^^^^^

.. java:method:: public void setParseInfo(Lattice lattice, FindContext<List<IrregularNode>> irregularFindContext, char jaso, int curIndex)
   :outertype: IrregularParser

