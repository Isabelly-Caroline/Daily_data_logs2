<<<<<<< HEAD
Hoje finalizei a instalação do Python e do PySpark, além de configurar o ambiente no VS Code e criar um ambiente virtual (venv). Depois disso fiz alguns testes para garantir que estava certo. 

Durante o estudo foquei em entender os conceitos iniciais da linguagem e me familiarizar com a sintaxe. Bom hoje os pontos que eu estudei foram o SparkSession, DataFrames, criação de DataFrames e algumas operações simples como filtros utilizando filter() e visualização de resultados com show(). Também fiz comparações entre PySpark e SQL, que é uma linguagem que eu já tenho mais familiaridade, o que ajudou bastante a entender a lógica das operações.

Na prática para treinar executei um exemplo simples criando um DataFrame e aplicando um filtro nos dados:

```python id="4m55gb"
from pyspark.sql import SparkSession

spark = SparkSession.builder.appName("Desafio1").getOrCreate()

dados = [
("Ana",17,8),
("Carlos",19,6),
("Marina",18,9),
("João",20,5)
]

df = spark.createDataFrame(dados, ["nome","idade","nota"])

df.filter(df.nota > 7).show()

spark.stop()
```

Hoje preferi estudar mais por conta própria e focar na prática, testando exemplos e explorando a linguagem, então não fiz o curso em si. Comparar com SQL também ajudou bastante a entender o estilo do PySpark. Amanhã provavelmente volto ao curso, mas pretendo seguir praticando e explorando exemplos para ir fixando melhor.
=======
# Daily_data_logs
>>>>>>> ff888ed4e1554f9b2829831ed118684fe6ba0efd
