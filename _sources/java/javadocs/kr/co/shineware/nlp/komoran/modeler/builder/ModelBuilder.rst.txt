.. java:import:: kr.co.shineware.nlp.komoran.constant FILENAME

.. java:import:: kr.co.shineware.nlp.komoran.constant SYMBOL

.. java:import:: kr.co.shineware.nlp.komoran.corpus.model Dictionary

.. java:import:: kr.co.shineware.nlp.komoran.corpus.model Grammar

.. java:import:: kr.co.shineware.nlp.komoran.model ScoredTag

.. java:import:: kr.co.shineware.nlp.komoran.parser KoreanUnitParser

.. java:import:: kr.co.shineware.util.common.file FileUtil

.. java:import:: kr.co.shineware.util.common.model Pair

.. java:import:: java.io BufferedReader

.. java:import:: java.io File

.. java:import:: java.io FileReader

.. java:import:: java.util Map.Entry

ModelBuilder
============

.. java:package:: kr.co.shineware.nlp.komoran.modeler.builder
   :noindex:

.. java:type:: public class ModelBuilder

   코퍼스 빌드 결과물로 모델 생성 생성되는 데이터는 아래와 같음 - 관측 확률(observation.model) - 전이 확률(transition.model) - 불규칙 모델(irregular.model) - 품사 테이블(pos.table)

   :author: Junsoo Shin

Methods
-------
buildPath
^^^^^^^^^

.. java:method:: public void buildPath(String path)
   :outertype: ModelBuilder

   입력된 path에 저장된 데이터로 부터 model 빌드  path 내에는 아래와 같은 데이터들이 포함되어 있어야함  - 단어 사전 파일 : dic.word - 불규칙 사전 파일 : dic.irregular - 품사 간 문법 사전 : grammar.in

   :param path: 모델을 생성하기 위한 트레이닝 데이터 위치

load
^^^^

.. java:method:: @Deprecated public void load(String path)
   :outertype: ModelBuilder

save
^^^^

.. java:method:: public void save(String path)
   :outertype: ModelBuilder

   build된 모델들(transition, observation, pos_table)을 path 폴더에 저장

   :param path:

setExternalDic
^^^^^^^^^^^^^^

.. java:method:: public void setExternalDic(String externalDic)
   :outertype: ModelBuilder

