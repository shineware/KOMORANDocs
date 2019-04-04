.. java:import:: kr.co.shineware.ds.aho_corasick FindContext

.. java:import:: kr.co.shineware.nlp.komoran.constant SYMBOL

.. java:import:: kr.co.shineware.nlp.komoran.model ScoredTag

.. java:import:: java.util List

.. java:import:: java.util Map

.. java:import:: java.util Set

RegularParser
=============

.. java:package:: kr.co.shineware.nlp.komoran.core.model
   :noindex:

.. java:type:: public class RegularParser implements Parser

Constructors
------------
RegularParser
^^^^^^^^^^^^^

.. java:constructor:: public RegularParser(Resources resources)
   :outertype: RegularParser

Methods
-------
parse
^^^^^

.. java:method:: @Override public void parse()
   :outertype: RegularParser

setParseInfo
^^^^^^^^^^^^

.. java:method:: public void setParseInfo(Lattice lattice, FindContext<List<ScoredTag>> observationFindContext, char jaso, int curIndex)
   :outertype: RegularParser

