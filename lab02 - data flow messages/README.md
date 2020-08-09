# Modelo para Apresentação do Lab02 - Data Flow & Mensagens

## Tarefa sobre catálogo de componentes

[Exercícios - catálogo de componentes](https://github.com/jhowmerisse/INF331-labs/blob/master/lab02%20-%20data%20flow%20messages/notebook/components-01-catalog.ipynb)

## Tarefa Web Components 1

~~~html
<dcc-trigger label="Mundo"
             action="noticia/mundo/politica"
             value="nova notícia sobre política no mundo">
</dcc-trigger>

<dcc-trigger label="Brasil P"
             action="noticia/brasil/politica"
             value="nova notícia sobre política no Brasil">
</dcc-trigger>

<dcc-trigger label="Brasil E"
             action="noticia/brasil/esporte"
             value="nova notícia sobre esporte no Brasil">
</dcc-trigger>

<dcc-trigger label="Bahia"
             action="noticia/bahia/esporte"
             value="nova notícia sobre esporte na Bahia">
</dcc-trigger>

<dcc-lively-talk
                 character="doctor"
                 speech="..."><subscribe-dcc topic="#/politica"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk
                 character="nurse"
                 speech="..."><subscribe-dcc topic="+/b#"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk
                 character="patient"
                 speech="..."><subscribe-dcc topic="noticia/#"></subscribe-dcc>
</dcc-lively-talk>
~~~

## Tarefa Web Components 2

~~~html
<dcc-trigger label="start Process" action="next/rss">
</dcc-trigger>

<dcc-rss publish="rss/science" source="https://www.wired.com/category/science/feed">
  <subscribe-dcc topic="next/rss" role="start"></subscribe-dcc>
</dcc-rss>

<dcc-rss publish="rss/design" source="https://www.wired.com/category/design/feed">
  <subscribe-dcc topic="next/rss" role="start"></subscribe-dcc>
</dcc-rss>

<dcc-aggregator publish="aggregate/science" quantity="3">
  <subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-aggregator>

<dcc-lively-talk 
                 character="doctor"
                 speech="...">
  <subscribe-dcc topic="aggregate/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk 
                 character="nurse"
                 speech="...">
  <subscribe-dcc topic="rss/science"></subscribe-dcc>
</dcc-lively-talk>

<dcc-lively-talk 
                 character="patient"
                 speech="...">
  <subscribe-dcc topic="rss/design"></subscribe-dcc>
</dcc-lively-talk>
~~~
