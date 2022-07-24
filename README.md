# Predição de Alta Hospitalar empregando hemograma e Random Forest

**Objetivos gerais:** Obter modelos de predição sobre a alta hospitalar e verificar se esses modelos são distintos considerando os gêneros masculino e feminino.

**Base de dados**

Para esta implementação foi utilizada base de dados disponilizada por Sadikin, Mujiono (2020), “EHR Dataset for Patient Treatment Classification”, Mendeley Data, V1, doi: 10.17632/7kv3rctx7m.1

Ela é composta das seguintes variáveis

<table>
<thead>
<tr><td>Nome</td><td>Tipo</td><td>Descrição</td></tr>
</thead>
<tbody>
<tr><td>HAEMATOCRIT</td><td>Contínua</td><td>Contagem de eritrócitos multiplicado pelo VCM</td></tr>
<tr><td>HAEMOGLOBINS</td><td>Contínua</td><td>Dosagem de hemoglobina</td></tr>
<tr><td>ERYTHROCYTE</td><td>Contínua</td><td>Contagem de eritrócitos</td></tr>
<tr><td>LEUCOCYTE</td><td>Contínua</td><td>Contagem de leucócitos</td></tr>
<tr><td>THROMBOCYTE</td><td>Contínua</td><td>Contagem de plaquetas.</td></tr>
<tr><td>MCH</td><td>Contínua</td><td>Hemoglobina Corpuscular média</td></tr>
<tr><td>MCHC</td><td>Contínua</td><td>Concentração de Hemoglobina Corpuscular Média</td></tr>
<tr><td>MCV</td><td>Contínua</td><td>Volume Corpuscular Médio (VCM)</td></tr>
<tr><td>AGE</td><td>Contínua</td><td>Idade do paciente.</td></tr>
<tr><td>SEX</td><td>Nominal (F ou M)</td><td>Gênero do paciente.</td></tr>
<tr><td>SOURCE</td><td>Nominal (in ou out)</td><td>Classe de cada amostra. "in": atendimento hospitalar, "out": atendimento externo.</td></tr>
</tbody>
</table>

* Na implementação realizada na pesquisa "Exploratory Study of Some Machine Learning Techniques to Classify the Patient Treatment" empregaram vários algoritmos, e constataram que o XGBoost gerou os melhores resultados, tendo obtido uma acurácia máxima de 0.7579.

* Aqui faremos uma abordagem distinta, pois a base de dados será separada por gênero, ou seja, os atributos do gênero masculino serão utilizados separadamento daqueles do gênero feminino para obter os modelos de predição. Isso é motivado pelo fato que os valores de referência dos exames são distintos dependendo do gênero. Além disso empregaremos o algoritmo Random Forest, pois tem menor custo computacional na fase ade aprendizado.

**Para mais detalhes e discussão sobre o assunto acesse o capítulo de e-book: "Um modelo de Inteligência Artificial para auxílio na
decisão de alta hospitalar"** disponível aqui: https://editorapantanal.com.br/ebooks-capitulo.php?ebook_id=topicos-nas-ciencias-da-saude-volume-ix&ebook_ano=2022&ebook_caps=1&ebook_capitulo=Cap13&ebook_org=1

**Acesse este vídeo-tutorial pelo Youtube:** https://www.youtube.com/watch?v=cTCoBIBPJSc
