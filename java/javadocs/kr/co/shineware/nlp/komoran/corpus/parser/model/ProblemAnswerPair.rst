.. java:import:: java.util List

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser CorpusParser

.. java:import:: kr.co.shineware.util.common.model Pair

ProblemAnswerPair
=================

.. java:package:: kr.co.shineware.nlp.komoran.corpus.parser.model
   :noindex:

.. java:type:: public class ProblemAnswerPair

   \ :java:ref:`CorpusParser`\ 에 사용되는 model형태의 클래스로써 get,set 메소드만 존재함  problem은 원본 데이터를 지칭하며, answer는 원본 데이터의 분석된 결과(태깅된 결과)를 지칭함

   :author: Junsoo Shin

Methods
-------
getAnswer
^^^^^^^^^

.. java:method:: public String getAnswer()
   :outertype: ProblemAnswerPair

getAnswerList
^^^^^^^^^^^^^

.. java:method:: public List<Pair<String, String>> getAnswerList()
   :outertype: ProblemAnswerPair

getProblem
^^^^^^^^^^

.. java:method:: public String getProblem()
   :outertype: ProblemAnswerPair

setAnswer
^^^^^^^^^

.. java:method:: public void setAnswer(String answer)
   :outertype: ProblemAnswerPair

setAnswerList
^^^^^^^^^^^^^

.. java:method:: public void setAnswerList(List<Pair<String, String>> answerList)
   :outertype: ProblemAnswerPair

setProblem
^^^^^^^^^^

.. java:method:: public void setProblem(String problem)
   :outertype: ProblemAnswerPair

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: ProblemAnswerPair

