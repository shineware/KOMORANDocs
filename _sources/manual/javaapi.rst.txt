.. KOMORANDocs documentation master file, created by
   sphinx-quickstart on Tue Feb 26 22:28:06 2019.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Java API
=======================================

본 문서에서는 Komoran에서 제공되는 다양한 API 들에 대해서 살펴봅니다.

Komoran
---------------------------------------

.. code-block:: java

 public Komoran(String modelPath)

Komoran 생성자 입니다. 모델 경로를 인자로 받으며 Komoran 생성 시 해당 모델을 로드합니다.


.. code-block:: java

  public Komoran(DEFAULT_MODEL modelType)

Komoran 생성자 입니다. 기본으로 제공하는 모델을 선택하여 생성합니다. DEFAULT_MODEL.LIGHT와 DEFAULT_MODEL.FULL의 두 가지 버전을 기본적으로 제공합니다.


.. code-block:: java

  void setFWDic(String filename)

기분석 사전을 로드합니다. 기분석 사전의 경로를 인자로 받습니다.

.. code-block:: java

  void setUserDic(String userDic)

사용자 사전을 로드합니다. 사용자 사전의 경로를 인자로 받습니다.

.. code-block:: java

  KomoranResult analyze(String sentence)

입력 문장에 대한 형태소 분석을 수행합니다. 입력 문장에 대한 형태소 분석 결과를 KomoranResult 객체로 반환합니다.

.. code-block:: java

  void analyzeTextFile(String inputFilename, String outputFilename, int thread)

파일 단위로 형태소 분석을 수행합니다. 형태소 분석이 필요한 파일의 경로, 형태소 분석 결과가 출력될 파일의 경로, 분석 시 사용할 쓰레드 수를 인자로 받습니다.

.. code-block:: java

  List<KomoranResult> analyze(List<String> sentences, int thread)

여러 문장에 대한 형태소 분석을 수행합니다. 분석할 문장의 List, 분석 시 사용할 쓰레드 수를 인자로 받습니다. 분석된 결과는 List<KomoranResult>로 반환됩니다.

.. code-block:: java

  List<KomoranResult> analyze(String sentence, int nbest)

입력 문장에 대한 형태소 분석 결과 중 n-best를 제공합니다. 분석할 문장, n-best를 인자로 받습니다. n-best 만큼의 형태소 분석 결과를 List<KomoranResult>로 반환합니다.


KomoranResult
---------------------------------------

.. code-block:: java

  List<LatticeNode> getResultNodeList()

형태소분석 결과를 List<LatticeNode> 형태로 반환합니다.

.. code-block:: java

  public List<String> getNouns()

형태소 분석 결과 중 명사류를 List<String> 형태로 반환합니다.

.. code-block:: java

  public List<String> getMorphesByTags(String... str)

형태소 분석 결과 중 특정 품사에 해당하는 형태소만 반환합니다.

.. code-block:: java

  public List<String> getMorphesByTags(Collection<String> targetPosCollection)

형태소 분석 결과 중 특정 품사에 해당하는 형태소만 반환합니다.

.. code-block:: java

  public String getPlainText()

형태소 분석 결과를 plain text형태의 string으로 반환합니다.

.. code-block:: java

  public List<Token> getTokenList()

형태소 분석 결과를 List<Token> 형태로 반환합니다. Token에는 형태소, 품사, 시작 위치, 끝나는 위치 등의 정보를 포함하고 있습니다.

.. code-block:: java

  public List<Pair<String, String>> getList()

형태소 분석 결과를 형태소, 품사 Pair의 리스트 형태로 반환합니다.


CorpusBuilder
---------------------------------------

.. code-block:: java

  public void save(String savePathName)

빌드한 코퍼스를 savePathName 경로에 저장합니다. savePathName 밑에 ``dic.irregular``, ``dic.word``, ``grammar.in`` 파일이 저장됩니다.

.. code-block:: java

  public void load(String loadPath)

빌드된 코퍼스를 load 합니다. loadPath 디렉토리 아래에는 save를 통해 생성된 ``dic.irregular``, ``dic.word``, ``grammar.in`` 파일이 있어야합니다.


.. code-block:: java

  public void buildPath(String corporaPath)

corporaPath 밑에 있는 모든 파일을 빌드합니다. 서브디렉토리에 있는 모든 파일들을 대상으로 합니다.

.. code-block:: java

  public void buildPath(String corporaPath, String suffix)

corporaPath 밑에 있는 모든 파일 중 파일 확장자가 suffix로 끝나는 파일들만 빌드합니다.

.. code-block:: java

  public void build(String filename)

filename에 해당하는 파일을 빌드합니다.

.. code-block:: java

  public void appendUserDic(String filename)

filename에 해당하는 사용자 사전을 추가하여 코퍼스 빌드 시 함께 빌드됩니다.

.. code-block:: java

  public void appendUserDicPath(String path, String suffix)

path 밑에 있는 모든 파일 중 확장자가 suffix로 끝나는 파일들만 사용자 사전으로 추가하여 코퍼스 빌드 시 함께 빌드됩니다.


ModelBuilder
---------------------------------------

.. code-block:: java

  public void setExternalDic(String externalDic)

``본 메소드는 반드시 buildPath 메소드 호출 전에만 사용가능합니다.``
externalDic 경로에 있는 외부 사전을 추가하여 모델을 빌드합니다. 외부 사전에 등록된 단어들의 빈도수는 50으로 초기화되어 모델에 반영됩니다.

.. code-block:: java

  public void buildPath(String path)

입력된 path 디렉토리 내 저장된 파일로부터 model을 빌드합니다. path 내에는 ``dic.word``, ``dic.irregular``, ``grammar.in`` 파일이 포함되어 있어야 합니다.

.. code-block:: java

  public void save(String path)

``본 메소드 호출 전에 반드시 buildPath 메소드를 실행해야 합니다``
빌드된 모델을 path 디렉토리에 저장합니다. path 디렉토리에는 ``irregular.model``, ``observation.model``, ``pos.table``, ``transition.model`` 파일이 생성됩니다.
