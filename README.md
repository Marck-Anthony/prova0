# prova0
Atividade Prática 1.2: Implementação e Governança
```markdown
# Visão Computacional com Python e OpenCV

Este repositório contém a implementação dos exercícios e conceitos fundamentais do livro **"Introdução à Visão Computacional com Python e OpenCV"**, adaptados para execução no ambiente **Google Colab**.

O projeto aborda desde a manipulação básica de pixels até técnicas de filtragem, histogramas e segmentação de imagens.

## 🚀 Como Executar no Google Colab

Para facilitar a execução sem a necessidade de configurar um ambiente local, você pode abrir o projeto diretamente no Google Colab clicando no botão abaixo:

[![Open In Colab](https://colab.research.google.com/drive/1GiBlEzF6rEf3Ec239kHeKWwwLh_in5EJ?usp=sharing)
---

## 🛠️ Instalação e Requisitos

Caso prefira rodar o projeto localmente (em sua máquina), você precisará do Python instalado e deverá executar o seguinte comando para instalar as dependências necessárias:

```bash
pip install opencv-python numpy matplotlib
```

*Nota: No Google Colab, essas bibliotecas já vêm pré-instaladas por padrão.*

---

## ⚙️ Configurações Necessárias

Para que o código funcione corretamente, siga estas diretrizes:

### 1. Ajuste para Exibição de Imagens
No ambiente Colab, a função padrão `cv2.imshow()` está desabilitada pois causa o travamento da sessão. Em todas as células, utilizamos o patch específico:
```python
from google.colab.patches import cv2_imshow
# Use cv2_imshow(imagem) em vez de cv2.imshow('janela', imagem)
```

### 2. Clonando o Repositório Inteiro
Se você tiver muitas imagens em uma pasta, é mais rápido clonar o repositório todo de uma vez.

```python
!git clone https://github.com/Marck-Anthony/prova0.git
Após rodar isso, o Colab criará uma pasta com o nome do repositório.
```
Para acessar as imagens, use o caminho: '/content/prova0/img/1.png'.

---

## 📂 Organização do Notebook

O arquivo `prova0.ipynb` está organizado da seguinte forma:

* **Manipulação de Pixels:** Acesso a coordenadas, fatiamento (slicing) e alteração de cores.
* **Espaços de Cores:** Conversões para Tons de Cinza e HSV, além da separação de canais BGR.
* **Transformações Geométricas:** Redimensionamento (resize) e Recorte (ROI).
* **Aritmética e Máscaras:** Adição de brilho (`cv2.add`) e aplicação de máscaras bitwise.
* **Histogramas:** Cálculo, plotagem e equalização para melhoria de contraste.
* **Thresholding:** Binarização simples para segmentação de objetos.

---

## ✍️ Autoria
Desenvolvido como parte da primeira prova da disciplina Processamento de Imagem.
