.. java:import:: kr.co.shineware.nlp.komoran.constant DEFAULT_MODEL

.. java:import:: kr.co.shineware.nlp.komoran.constant FILENAME

.. java:import:: kr.co.shineware.nlp.komoran.constant SCORE

.. java:import:: kr.co.shineware.nlp.komoran.constant SYMBOL

.. java:import:: kr.co.shineware.nlp.komoran.core.model ContinuousSymbolBuffer

.. java:import:: kr.co.shineware.nlp.komoran.core.model Lattice

.. java:import:: kr.co.shineware.nlp.komoran.core.model LatticeNode

.. java:import:: kr.co.shineware.nlp.komoran.core.model Resources

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser CorpusParser

.. java:import:: kr.co.shineware.nlp.komoran.corpus.parser.model ProblemAnswerPair

.. java:import:: kr.co.shineware.nlp.komoran.model KomoranResult

.. java:import:: kr.co.shineware.nlp.komoran.model MorphTag

.. java:import:: kr.co.shineware.nlp.komoran.model ScoredTag

.. java:import:: kr.co.shineware.nlp.komoran.modeler.model IrregularNode

.. java:import:: kr.co.shineware.nlp.komoran.modeler.model Observation

.. java:import:: kr.co.shineware.nlp.komoran.parser KoreanUnitParser

.. java:import:: kr.co.shineware.nlp.komoran.util KomoranCallable

.. java:import:: kr.co.shineware.util.common.file FileUtil

.. java:import:: kr.co.shineware.util.common.model Pair

.. java:import:: kr.co.shineware.util.common.string StringUtil

.. java:import:: java.util.concurrent Executors

.. java:import:: java.util.concurrent Future

.. java:import:: java.util.concurrent ThreadPoolExecutor

Komoran
=======

.. java:package:: kr.co.shineware.nlp.komoran.core
   :noindex:

.. java:type:: public class Komoran implements Cloneable

Constructors
------------
Komoran
^^^^^^^

.. java:constructor:: public Komoran(String modelPath)
   :outertype: Komoran

Komoran
^^^^^^^

.. java:constructor:: public Komoran(DEFAULT_MODEL modelType)
   :outertype: Komoran

Methods
-------
analyze
^^^^^^^

.. java:method:: public List<KomoranResult> analyze(List<String> sentences, int thread)
   :outertype: Komoran

analyze
^^^^^^^

.. java:method:: public KomoranResult analyze(String sentence)
   :outertype: Komoran

analyze
^^^^^^^

.. java:method:: public List<KomoranResult> analyze(String sentence, int nbest)
   :outertype: Komoran

analyzeTextFile
^^^^^^^^^^^^^^^

.. java:method:: public void analyzeTextFile(String inputFilename, String outputFilename, int thread)
   :outertype: Komoran

load
^^^^

.. java:method:: public void load(String modelPath)
   :outertype: Komoran

setFWDic
^^^^^^^^

.. java:method:: public void setFWDic(String filename)
   :outertype: Komoran

setUserDic
^^^^^^^^^^

.. java:method:: public void setUserDic(String userDic)
   :outertype: Komoran

