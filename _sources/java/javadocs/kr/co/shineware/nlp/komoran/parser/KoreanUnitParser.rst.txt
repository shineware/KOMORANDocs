.. java:import:: kr.co.shineware.nlp.komoran.interfaces UnitParser

.. java:import:: kr.co.shineware.util.common.model Pair

.. java:import:: java.lang Character.UnicodeBlock

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

KoreanUnitParser
================

.. java:package:: kr.co.shineware.nlp.komoran.parser
   :noindex:

.. java:type:: public class KoreanUnitParser implements UnitParser

Fields
------
ChoSung
^^^^^^^

.. java:field:: public static char[] ChoSung
   :outertype: KoreanUnitParser

JongSung
^^^^^^^^

.. java:field:: public static char[] JongSung
   :outertype: KoreanUnitParser

JungSung
^^^^^^^^

.. java:field:: public static char[] JungSung
   :outertype: KoreanUnitParser

Methods
-------
combine
^^^^^^^

.. java:method:: @Override public String combine(String str)
   :outertype: KoreanUnitParser

combineWithType
^^^^^^^^^^^^^^^

.. java:method:: public String combineWithType(List<Pair<Character, UnitType>> jasoUnitsWithType)
   :outertype: KoreanUnitParser

getSyllableAreaList
^^^^^^^^^^^^^^^^^^^

.. java:method:: public List<Pair<Integer, Integer>> getSyllableAreaList(String str)
   :outertype: KoreanUnitParser

parse
^^^^^

.. java:method:: @Override public String parse(String str)
   :outertype: KoreanUnitParser

parseWithType
^^^^^^^^^^^^^

.. java:method:: public List<Pair<Character, UnitType>> parseWithType(String str)
   :outertype: KoreanUnitParser

