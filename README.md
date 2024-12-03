# Transformando Imagens com Python  

Este projeto oferece uma maneira simples e prática de processar imagens usando Python. Ele realiza duas conversões básicas:  
1. **Tons de cinza:** transforma as cores de uma imagem em valores de cinza (escala de 0 a 255).  
2. **Binarização:** transforma a imagem em preto e branco (valores 0 ou 255), com base em um limite de luminosidade.  

Tudo isso é feito com o auxílio da biblioteca **Pillow (PIL)**, amplamente utilizada para manipulação de imagens.  

---

## O que o código faz?  

1. **Converte uma imagem para texto**  
   Ele lê cada pixel da imagem e salva os valores RGB (vermelho, verde, azul) em um arquivo de texto (`entrada.txt`). Isso é útil para visualizar os dados "brutos" da imagem.  

2. **Converte para tons de cinza**  
   Um cálculo simples (média dos valores RGB) transforma a imagem original em escala de cinza.  

3. **Converte para binária (preto e branco)**  
   A imagem em tons de cinza é analisada, e cada pixel é comparado a um limite (padrão: 128). Pixels mais claros se tornam brancos (255) e os mais escuros, pretos (0).  

4. **Exibe e salva os resultados**  
   As imagens processadas são salvas em arquivos (`saida_cinza.png` e `saida_binaria.png`) e exibidas automaticamente.  

---

## Pré-requisitos  

- **Python 3.x**  
- **Pillow (PIL):**  
  Para instalar, execute:  
  ```bash
  pip install pillow
  ```
