.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser.model ProblemAnswerPair

.. java:import:: kr.co.shineware.nlp.komoran.exception FileFormatException

.. java:import:: kr.co.shineware.util.common.model Pair

.. java:import:: kr.co.shineware.util.common.string StringUtil

IrregularParser
===============

.. java:package:: kr.co.shineware.nlp.komoran.corpus.parser
   :noindex:

.. java:type:: public class IrregularParser

   불규칙 어휘 분석을 위한 parser  교착어 전용

   :author: Junsoo Shin

Methods
-------
parse
^^^^^

.. java:method:: public List<Pair<String, String>> parse(String problem, List<Pair<String, String>> answerList)
   :outertype: IrregularParser

   입력된 problem(어절)과 answerList(형태소, 품사)를 비교하여 변화가 일어나는 구간을 pair형태로 반환  problem과 answerList의 형태소는 자소 단위로 구성되어 있어야함

   :param problem:
   :param answerList:

parse
^^^^^

.. java:method:: public List<Pair<String, String>> parse(String line)
   :outertype: IrregularParser

parse
^^^^^

.. java:method:: public List<Pair<String, String>> parse(ProblemAnswerPair pair)
   :outertype: IrregularParser

