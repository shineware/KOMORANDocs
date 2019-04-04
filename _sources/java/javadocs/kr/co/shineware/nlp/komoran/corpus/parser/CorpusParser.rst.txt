.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: kr.co.shineware.nlp.komoran.corpus.builder CorpusBuilder

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser.model ProblemAnswerPair

.. java:import:: kr.co.shineware.nlp.komoran.exception FileFormatException

.. java:import:: kr.co.shineware.util.common.model Pair

CorpusParser
============

.. java:package:: kr.co.shineware.nlp.komoran.corpus.parser
   :noindex:

.. java:type:: public class CorpusParser

   \ :java:ref:`CorpusBuilder`\ 에 사용되는 파서로써 아래와 같은 형태로 이루어져 있는 경우에 사용 가능함 감기는 감기/NNG 는/JKG  자세한 내용은 아래 링크 참조 \ ` www.shineware.co.kr > FAQ > CorpusBuiler  <http://www.shineware.co.kr>`_\

   :author: Junsoo Shin

Methods
-------
parse
^^^^^

.. java:method:: public ProblemAnswerPair parse(String line) throws FileFormatException
   :outertype: CorpusParser

   입력된 라인을 파싱하여 \ :java:ref:`ProblemAnswerPair`\  형태로 반환

   :param line:
   :throws FileFormatException:

