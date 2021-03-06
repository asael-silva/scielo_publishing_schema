.. _elemento-funding-source:
 
<funding-source>
^^^^^^^^^^^^^^^^

Aparece em
  :ref:`elemento-award-group`
 
Ocorre
  Uma ou mais vezes


Esta tag deve ficar dentro de :ref:`elemento-award-group` e nela será 
especificado o órgão e/ou instituição financiadora:
 
Exemplo:

.. code-block:: xml
 
    ...
    <article-meta>
        ...
        <funding-group>           
            <award-group>
                <funding-source>CNPq</funding-source>
                <award-id>1685X6-7</award-id>
            </award-group>
        </funding-group>
        ...
    </article-meta>
    ...
 

Existem casos em que há mais que uma instituição financiadora para um único 
número de contrato.

Exemplo:

.. code-block:: xml

    ...
    <article-meta>
       ...
       <funding-group>
          <award-group>
             <funding-source>CNPq</funding-source>
             <funding-source>FAPESP</funding-source>
             <award-id>#09/06953-4</award-id>
          </award-group>
       </funding-group>
       ...
    </article-meta>
    ...
