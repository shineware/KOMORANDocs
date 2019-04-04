.. java:import:: java.io BufferedWriter

.. java:import:: java.io FileWriter

.. java:import:: java.io IOException

.. java:import:: java.util HashMap

.. java:import:: java.util List

.. java:import:: java.util Map

.. java:import:: java.util Map.Entry

.. java:import:: java.util Set

.. java:import:: kr.co.shineware.nlp.komoran.interfaces FileAccessible

.. java:import:: kr.co.shineware.util.common.file FileUtil

.. java:import:: kr.co.shineware.util.common.string StringUtil

Grammar
=======

.. java:package:: kr.co.shineware.nlp.komoran.corpus.model
   :noindex:

.. java:type:: public class Grammar implements FileAccessible

   This is model class of grammar. Grammar class implements {@FileAccessible}. Therefore, this is can use like DB instead of save, load.

   :author: Junsoo Shin

   **See also:** :java:ref:`{@linkFileAccessible}`

Constructors
------------
Grammar
^^^^^^^

.. java:constructor:: public Grammar()
   :outertype: Grammar

   문법 생성자

Grammar
^^^^^^^

.. java:constructor:: public Grammar(String filename)
   :outertype: Grammar

   문법 생성자로써 filename에 저장되어 있는 grammar를 로드

   :param filename:

Methods
-------
append
^^^^^^

.. java:method:: public void append(String prevPos, String nextPos)
   :outertype: Grammar

   grammar에 prevPos to nextPos 문법 추가 기존에 존재하는 문법이면 문법의 출현 빈도수를 1만큼 증가 시킴

   :param prevPos:
   :param nextPos:

getGrammar
^^^^^^^^^^

.. java:method:: public Map<String, Map<String, Integer>> getGrammar()
   :outertype: Grammar

   현재 메모리에 있는 grammar를 반환 Map> 형태로 구성되어 있음

has
^^^

.. java:method:: public boolean has(String prevPos, String nextPos)
   :outertype: Grammar

   현재 grammar에 존재하는 문법인지 검사

   :param prevPos:
   :param nextPos:

load
^^^^

.. java:method:: @Override public void load(String filename)
   :outertype: Grammar

save
^^^^

.. java:method:: @Override public void save(String filename)
   :outertype: Grammar

