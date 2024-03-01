# LabIa-900
Aprendizado de máquina automatizado para previsão de aluguel de bicicletas


1º Passo criado conta em Azure 

2º Passo cliquei em Azure Machine Learning Studio .

3º Criei um novo trabalho de Machine Learn  com as seguintes configurações :

4º Passo nas configuraçoes basicas coloquei : 

O Nome do trabalho : mslearn-bike-automl
O Novo nome do experimento : mslearn-bike-rental
Na Descrição : Aprendizado de máquina automatizado para previsão de aluguel de bicicletas
Os Marcadores : nenhum

5º Passo no Tipo de tarefa e dados :

selecionei o tipo de tarefa como Regressão
No conjunto de dados criei um novo conjunto de dados com as seguintes configurações:
Nome : aluguel de bicicletas
Descrição : dados históricos de aluguel de bicicletas
Tipo : Tabular


6º Passo na Fonte de dados :
Selecionei  arquivos da web
Coloquei a url : https://aka.ms/bike-rentals
Ignorar validação de dados : não selecionei


7º Passo nas Configurações :
Formato de arquivo : Delimitado
Delimitador : Vírgula
Codificação : UTF-8
Cabeçalhos de coluna : apenas o primeiro arquivo possui cabeçalhos
Pular linhas : Nenhum
O conjunto de dados contém dados multilinhas : não selecionei 

8º no esquema : 
Incluir todas as colunas com exessão do caminho 
Selecionei Criar 

9º Passo na aba das configurações de tarefa :
O Tipo de tarefa é : Regressão
Conjunto de dados são : aluguel de bicicletas
Coluna de destino : Aluguéis (inteiro)


10 º Passo na aba de configurações adicionais :
Métrica primária : raiz do erro quadrático médio normalizado
Explique o melhor modelo : Não selecionado
Desmarcado o usar todos os modelos suportados  . 
Modelos permitidos : Selecionado apenas RandomForest e LightGBM .
Limites : expanda esta seção
Máximo de testes : 3
Máximo de testes simultâneos : 3
Máximo de nós : 3
Limite de pontuação da métrica : 0,085 
Tempo limite : 15
Tempo limite de iteração : 15
Habilitar rescisão antecipada : selecionei.

11º Passo na aba Validação e teste :
Tipo de validação : divisão de validação de trenamento
Porcentagem de dados de validação : 10
Conjunto de dados de teste : Nenhum

12º Passo na aba Calcular : 
Selecionei  o tipo de computação : e coloqueia a opção sem servidor
No tipo de máquina virtual : opção CPU
Na camada de máquina virtual calocada a opção : Dedicada
No tamanho da máquina virtual colocada a vesão :  Standard_DS3_V2*
Número de instâncias : 1
Colocado o trabalho de treinamento

