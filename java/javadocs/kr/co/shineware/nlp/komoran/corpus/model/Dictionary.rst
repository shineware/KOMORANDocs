.. java:import:: java.io BufferedReader

.. java:import:: java.io BufferedWriter

.. java:import:: java.io FileReader

.. java:import:: java.io FileWriter

.. java:import:: java.io IOException

.. java:import:: java.util HashMap

.. java:import:: java.util List

.. java:import:: java.util Map

.. java:import:: java.util Map.Entry

.. java:import:: java.util Set

.. java:import:: kr.co.shineware.nlp.komoran.interfaces FileAccessible

.. java:import:: kr.co.shineware.util.common.collection MapUtil

Dictionary
==========

.. java:package:: kr.co.shineware.nlp.komoran.corpus.model
   :noindex:

.. java:type:: public class Dictionary implements FileAccessible

   This class is model of dictionary. It can be used like DB instead of save, load.

   :author: Junsoo Shin

Constructors
------------
Dictionary
^^^^^^^^^^

.. java:constructor:: public Dictionary()
   :outertype: Dictionary

   사전 생성자로써 init() method 실행.

Dictionary
^^^^^^^^^^

.. java:constructor:: public Dictionary(String filename)
   :outertype: Dictionary

   사전 생성자로써 filename에 저장된 사전 데이터를 로딩 데이터 로딩 시 init method 실행

   :param filename:

Methods
-------
append
^^^^^^

.. java:method:: public void append(String word, String pos)
   :outertype: Dictionary

   사전에 형태소, 품사를 추가  overwrite형식이 아닌 append 형식으로써 단어에 따른 품사의 빈도수를 증가시킴

   :param word:
   :param pos:

append
^^^^^^

.. java:method:: public void append(String word, String pos, int inc)
   :outertype: Dictionary

get
^^^

.. java:method:: protected List<String> get(String word)
   :outertype: Dictionary

   단어의 품사 리스트를 반환

   :param word:

getDictionary
^^^^^^^^^^^^^

.. java:method:: public Map<String, Map<String, Integer>> getDictionary()
   :outertype: Dictionary

   현재 메모리에 올라가 있는 사전 데이터를 반환.

getPosList
^^^^^^^^^^

.. java:method:: public List<String> getPosList(String word)
   :outertype: Dictionary

   단어의 품사 리스트를 반환

   :param word:

init
^^^^

.. java:method:: protected void init()
   :outertype: Dictionary

   사전이 사용되는 메모리 초기화. 내부적으로 Double Map collection 사용됨.

load
^^^^

.. java:method:: @Override public void load(String filename)
   :outertype: Dictionary

save
^^^^

.. java:method:: @Override public void save(String filename)
   :outertype: Dictionary

