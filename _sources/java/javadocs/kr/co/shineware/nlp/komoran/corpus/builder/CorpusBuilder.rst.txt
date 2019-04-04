.. java:import:: kr.co.shineware.nlp.komoran.constant FILENAME

.. java:import:: kr.co.shineware.nlp.komoran.constant SYMBOL

.. java:import:: kr.co.shineware.nlp.komoran.corpus.model Dictionary

.. java:import:: kr.co.shineware.nlp.komoran.corpus.model Grammar

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser CorpusParser

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser IrregularParser

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser.model ProblemAnswerPair

.. java:import:: kr.co.shineware.nlp.komoran.exception FileFormatException

.. java:import:: kr.co.shineware.nlp.komoran.interfaces UnitParser

.. java:import:: kr.co.shineware.nlp.komoran.parser KoreanUnitParser

.. java:import:: kr.co.shineware.util.common.file FileUtil

.. java:import:: kr.co.shineware.util.common.model Pair

.. java:import:: kr.co.shineware.util.common.string StringUtil

.. java:import:: java.io BufferedReader

.. java:import:: java.io File

.. java:import:: java.io FileReader

.. java:import:: java.lang Character.UnicodeBlock

.. java:import:: java.util ArrayList

.. java:import:: java.util HashSet

.. java:import:: java.util List

.. java:import:: java.util Set

CorpusBuilder
=============

.. java:package:: kr.co.shineware.nlp.komoran.corpus.builder
   :noindex:

.. java:type:: public class CorpusBuilder

   코퍼스로부터 모델 생성 시 필요한 데이터 생성 생성되는 데이터는 아래와 같음 - 단어 사전(word dictionary) - 문법(grammar) - 기분석 사전(full word-phrase dictionary) - 불규칙 사전(irregular dictionary)

   :author: Junsoo Shin

Constructors
------------
CorpusBuilder
^^^^^^^^^^^^^

.. java:constructor:: public CorpusBuilder()
   :outertype: CorpusBuilder

Methods
-------
appendUserDic
^^^^^^^^^^^^^

.. java:method:: public void appendUserDic(String filename)
   :outertype: CorpusBuilder

appendUserDicPath
^^^^^^^^^^^^^^^^^

.. java:method:: public void appendUserDicPath(String path, String suffix)
   :outertype: CorpusBuilder

build
^^^^^

.. java:method:: public void build(String filename)
   :outertype: CorpusBuilder

   파일로부터 데이터 생성

   :param filename:

buildPath
^^^^^^^^^

.. java:method:: public void buildPath(String corporaPath)
   :outertype: CorpusBuilder

   코퍼스에 포함된 각 학습 파일로부터 데이터(단어 사전, 문법, 기분석 사전, 불규칙 사전) 생성

   :param corporaPath:

buildPath
^^^^^^^^^

.. java:method:: public void buildPath(String corporaPath, String suffix)
   :outertype: CorpusBuilder

   코퍼스에 포함된 각 학습 파일로부터 데이터(단어 사전, 문법, 기분석 사전, 불규칙 사전) 생성 파일 확장자가 suffix와 일치하는 파일만 이용

   :param corporaPath:
   :param suffix:

load
^^^^

.. java:method:: @Deprecated public void load(String loadPath)
   :outertype: CorpusBuilder

save
^^^^

.. java:method:: public void save(String savePathName)
   :outertype: CorpusBuilder

   빌드된 데이터(단어 사전, 문법, 기분석 사전, 불규칙 사전)를 savePath에 저장

   :param savePathName:

setExclusiveIrrRule
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setExclusiveIrrRule(String filename)
   :outertype: CorpusBuilder

