# Sistema de Recomendação por Similaridade de Imagens

Este projeto desenvolve um sistema de recomendação por imagens capaz de identificar a similaridade visual entre produtos. Em vez de depender de metadados textuais (como preço, marca ou modelo), o sistema foca em características visuais como formato, cor e textura para sugerir itens relacionados a um produto de busca.

O objetivo é simular como um usuário em um site de e-commerce poderia encontrar produtos visualmente semelhantes ao que ele está interessado, proporcionando uma experiência de descoberta mais intuitiva e focada na aparência do item.


## Aplicações

- **E-commerce:** Sugerir produtos visualmente similares a um item visualizado ou buscado.

- **Moda e Design:** Recomendar peças de vestuário, acessórios ou itens de decoração com estética semelhante.

- **Catálogos de Produtos:** Explorar coleções de produtos com base em sua aparência.


## Tecnologias Utilizadas

- **Python:** Linguagem principal para desenvolvimento.

- **Deep Learning:** Utilização de redes neurais para extração de características visuais.

- **Modelos de Classificação de Imagens:** Treinamento de uma rede neural (como as baseadas em ResNet, VGG, ou modelos pré-treinados como os do TensorFlow Hub) para aprender representações visuais.

- **Calculo de Similaridade:** Métricas como similaridade de cosseno para comparar as representações extraídas das imagens.

- **Google Colab:** Ambiente de desenvolvimento para treinamento e experimentação com GPUs gratuitas.

- **TensorFlow/Keras (ou PyTorch):** Frameworks de Deep Learning utilizados para construir e treinar o modelo.

- **NumPy:** Para operações numéricas eficientes.


## Estrutura de Pastas do Projeto


```
/sistema_recomendacao
├── /datasets
│   ├── /relogios
│   │   ├── relogio1.jpg
│   │   └── ...
│   ├── /camisetas
│   │   ├── camiseta1.jpg
│   │   └── ...
│   └── /sapatos
│       ├── sapato1.jpg
│       └── ...
└── README.md
```

## Como executar o código no Google Colab:

### 1. Prepare seu Dataset:

- Crie uma pasta no seu Google Drive chamada ```sistema_recomendacao```.

- Dentro dela, crie uma pasta ```dataset```.

- Dentro de ```dataset```, crie subpastas para cada categoria de produto que você tem (ex: ```relogios```, ```camisetas```, ```sapatos```).

- Coloque as imagens de cada categoria dentro da sua respectiva pasta.

### 2. Ajuste os Caminhos:

- Certifique-se de que ```DATASET_PATH``` no Célula 1 aponte corretamente para a sua pasta ```dataset```.

- No Célula 5, ajuste ```QUERY_IMAGE_PATH``` para o caminho de uma imagem específica do seu ```dataset``` que você queira usar como exemplo de busca.

### 3. Execute as Células:

- Execute as células do notebook em ordem.

- A Célula 1 instalará as bibliotecas e montará seu Drive.

- A Célula 2 carregará o modelo pré-treinado (ResNet50, que é excelente para extração de características).

- A Célula 3 processará todas as suas imagens, extraindo as características visuais. Este passo pode demorar dependendo do tamanho do seu dataset.

- As Células 4 e 5 demonstrarão como gerar recomendações e visualizar os resultados.


### 📜 Licença
Este projeto está licenciado sob a Licença MIT.

### 📫 Contato

Fique à vontade para visitar meu perfil no GitHub: [@cezarcorrea](https://github.com/cezarcorrea)

---
