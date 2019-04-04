.. java:import:: kr.co.shineware.nlp.komoran.core Komoran

.. java:import:: kr.co.shineware.nlp.komoran.model KomoranResult

.. java:import:: java.util.concurrent Callable

KomoranCallable
===============

.. java:package:: kr.co.shineware.nlp.komoran.util
   :noindex:

.. java:type:: public class KomoranCallable implements Callable<KomoranResult>

   Created by shin285 on 2017. 4. 4..

Constructors
------------
KomoranCallable
^^^^^^^^^^^^^^^

.. java:constructor:: public KomoranCallable(Komoran komoran, String input)
   :outertype: KomoranCallable

Methods
-------
call
^^^^

.. java:method:: @Override public KomoranResult call() throws Exception
   :outertype: KomoranCallable

