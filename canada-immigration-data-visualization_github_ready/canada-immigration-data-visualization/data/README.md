# Pasta data

Coloque aqui o arquivo de dados usado no projeto.

Arquivo esperado:

```text
imigrantes_canada.csv
```

No Google Colab, o notebook original lê o arquivo usando:

```python
df = pd.read_csv('/content/imigrantes_canada.csv')
```

Para executar localmente, uma alternativa é ajustar o caminho para:

```python
df = pd.read_csv('data/imigrantes_canada.csv')
```

Caso a licença da base permita, você pode versionar o CSV no GitHub. Caso contrário, mantenha apenas esta instrução.
