.. _elemento-product:

<product>
---------

Aparece em
  :ref:`elemento-article-meta`
 
Atributos obrigatórios  
  1. product-type
 
Ocorre
  Zero ou mais vezes


Em ``<product>`` devem ser inseridas as informações do produto resenhado. 
É importante salientar que esta tag só deverá ser utilizada quando 
:ref:`elemento-article` possuir o atributo ``@article-type="book-review"``.

Os valores possíveis para ``@product-type`` são: 

+-----------+---------------------------------+
| Valor     | Descrição                       |
+===========+=================================+
| article   | referência de artigo            |
+-----------+---------------------------------+
| book      | referência de livro             |
+-----------+---------------------------------+
| chapter   | referência de capítulo de livro |
+-----------+---------------------------------+
| other     | outros tipos                    |
+-----------+---------------------------------+
| software  | referência de software          |
+-----------+---------------------------------+

 

.. code-block:: xml

    ...
    <article-meta>
        ...
        <product product-type="book">
            <person-group person-group-type="author">
                <name>
                    <surname>ONFRAY</surname>
                    <given-names>Michel</given-names>
                </name>
            </person-group>
            <source>La comunidad filosófica: manifiesto por una universidad popular</source>
            <year>2008</year>
            <publisher-name>Gedisa</publisher-name>
            <publisher-loc>Barcelona</publisher-loc>
            <size units="pages">155</size>
            <isbn>9788497842525</isbn>                          
            <inline-graphic xlink:href="1234-5678-rctb-45-05-690-gf01.tif"/>
        </product>
        <history>
            ...
        </history>
        ...
    </article-meta>
    ...

 
.. note:: A ordem das tags é importante! A tag ``<product>`` deve estar 
          inserida antes de :ref:`elemento-history` ou depois de 
          :ref:`elemento-fpage`.
               
