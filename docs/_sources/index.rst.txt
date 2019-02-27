.. KOMORANDocs documentation master file, created by
   sphinx-quickstart on Tue Feb 26 22:28:06 2019.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

KOMORAN 문서
=======================================

KOMORAN [#f1]_ 은 Java로 개발된 한국어 형태소 분석기입니다.

.. Note::
   KOMORAN은 `Apache 2.0 License <https://www.apache.org/licenses/LICENSE-2.0>`_ 로 배포되고 있습니다.
   이는 누구나 자유롭게 다운로드 받아 부분 또는 전체를 개인적 또는 상업적 목적으로 이용할 수 있음을 뜻합니다.
   더 자세한 내용은 `Apache License <https://www.apache.org/licenses/>`_ 를 참고해주세요.

----

참고자료
---------------------------------------

KOMORAN 참고 자료
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
KOMORAN을 개발한 shineware에서 제공하는 참고자료입니다.

* `GitHub 저장소 <https://github.com/shin285/KOMORAN>`_ 에 바로 실행할 수 있는 소스 코드가 공개되어 있습니다.
* `shineware 홈페이지 <https://shineware.co.kr>`_ 에서 `KOMORAN 소개 및 데모 <https://www.shineware.co.kr/products/komoran/>`_ 를 확인하실 수 있습니다.
* `KOMORAN Slack <https://komoran.slack.com/join/shared_invite/MTc3NTMzMDQ1NTY5LTE0OTM4MjE5MzktNDE3NmQ4NDNkNw>`_ 에 방문하셔서 사용법과 팁 등을 공유해주세요.

그 외 참고 자료
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
사용자 분들께서 만들어주신 참고자료입니다.

* 간단히 실행해볼 수 있는 `Simple API Server <https://github.com/9bow/KOMORANRestAPIServer>`_ 를 사용해보실 수 있습니다.
* Python 버전의 `KOMORAN3Py <https://github.com/lovit/komoran3py>`_ 도 공개되어 있습니다.


개요
---------------------------------------

특징
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
* Pure Java
   100% Java로만 개발되었기 때문에 자바가 설치된 환경이라면 어디서든지 사용 가능합니다.
* 외부 라이브러리 독립적
   자체 제작한 Library들만을 사용하여 외부 Library와의 의존성 문제가 없습니다.
* 경량화
   자소 단위 처리, TRIE 사전 등으로 약 50MB 메모리 상에서도 동작 가능합니다.
* Easy to Use
   Library 적용 후 소스 코드 내 1줄만 추가하여 형태소 분석기를 사용할 수 있습니다.
* 사전 관리 용이
   일반 텍스트 파일의 형태로 구성되어 가독성이 높으며 바로 편집이 가능합니다.
* 새로운 분석 결과
   타 형태소 분석기와 달리 공백이 포함된 형태소 단위로 분석이 가능합니다.

분석 예시
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
* 아래는 `KOMORAN 데모 <https://www.shineware.co.kr/products/komoran/>`_ 를 이용한 분석 예시입니다.
* 입력 문장: `대한민국은 민주공화국이다.`

.. image:: _static/images/KOMORAN_Sample_01.png
   :width: 640 px
   :alt: KOMORAN 분석 예시 #1
   :align: center

* 입력 문장: `대한민국의 주권은 국민에게 있고, 모든 권력은 국민으로부터 나온다.`

.. image:: _static/images/KOMORAN_Sample_02.png
   :width: 640 px
   :alt: KOMORAN 분석 예시 #2
   :align: center



.. toctree::
   :maxdepth: 2
   :caption: 시작하기
   :name: toc

   /firststep/installation
   /firststep/tutorial
   /firststep/postypes


.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`


.. [#f1]
   한국어 형태소 분석기를 뜻하는 KOrean MORphical ANalyzer의 약자입니다.
