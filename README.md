<h3>Manipulação de Arquivos JSON com a Base de Dados do IRIS</h3>
<p align="justify">Clique <a href="https://github.com/aiquantumneuro/treinamento_e_predicao_com_json/blob/main/note.ipynb">aqui</a> para visualizar o código do notebook.</p>
<div align="justify">
<h4>Métodos Utilizados</h4>

<b>visualization_json_inline</b> (visualiza o arquivo JSON)
<ul>
<li>url_path: endereço do arquivo de leitura.</li>
<li>limit: número máximo de registros na visualização.</li>
</ul>

<b>getOutputTypesJSON</b> (captura os valores possíveis em uma determinada coluna)
<ul>
<li>url_path: endereço do arquivo de leitura.</li>
<li>output_column: nome da coluna que terá os seus tipos/valores únicos retornados.</li>
</ul>

<b>dataSeparationJSON</b> (separa os dados do arquivo entre dados de treinamento e dados de teste)
<ul>
<li>url_path: endereço do arquivo de leitura.</li>
<li>list_inputs: lista de strings com os nomes das colunas que irão compor as listas de entrada.</li>
<li>list_outputs: lista de strings com os nomes das colunas que irão compor as listas de saída.</li>
<li>training_percentage: percentual entre 0 (0%) e 1 (100%) na seleção das amostras que serão usadas nas listas de treinamento.</li>
<li>test_percentage: percentual entre 0 (0%) e 1 (100%) na seleção das amostras que serão usadas nas listas de teste.</li>
</ul>

<b>fit</b> (treina o modelo)
<ul>
<li>inputs: lista com as entradas do treinamento.</li>
<li>outputs: lista com as saídas do treinamento.</li>
<li>gamma: número real para a precisão na separação das saídas do treinamento, quanto maior o número mais precisa a separação e mais lento o processo.</li>
</ul>

<b>test</b> (testa o resultado do treino)
<ul>
<li>inputs: entradas que terão as suas saídas previstas.</li>
<li>outputs: saídas desejadas para comparação do teste.</li>
</ul>

<b>plotBAR</b> (exibe um gráfico de barras)
<ul>
<li>x: lista com os valores do eixo X.</li>
<li>y: lista com os valores do eixo Y.</li>
<li>x_label: descrição para os dados do eixo X.</li>
<li>y_label: descrição para os dados do eixo Y.</li>
<li>title: título descritivo do gráfico.</li>
<li>bar_values: se definido como True exibe os valores das colunas, caso contrário os oculta.</li>
</ul>

<p align="justify">Também poderá ser utilizado o método <b>predict</b> em produção que recebe a lista de entradas que será prevista.</p>
</div>
