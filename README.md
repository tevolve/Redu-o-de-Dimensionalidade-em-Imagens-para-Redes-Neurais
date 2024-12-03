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

  ---

## Como usar
Baixe o código
Salve o script como:
```bash
processador_imagens.py.
```

• Escolha uma imagem
Coloque a imagem no mesmo diretório do script e nomeie-a como sua_imagem.jpg (ou ajuste o caminho no código).

***Execute o script***
No terminal ou editor, execute:
```bash
python processador_imagens.py
```
**Resultados**

O arquivo entrada.txt terá os dados da imagem em texto.
As imagens processadas serão salvas como saida_cinza.png e saida_binaria.png.
As imagens também serão exibidas automaticamente.

## Personalizações
Alterar o limite de binarização
Por padrão, o limite para binarizar é 128. Para usar outro valor, altere esta linha no código:
```bash
imagem_binaria = binarizar(imagem_cinza, limite=100)
```

## Alterar a imagem de entrada
Basta trocar o nome da imagem nesta linha:
```bash
caminho_imagem = 'minha_nova_imagem.jpg'
```

## Tratamento de erros
**Se algo der errado:**

• Certifique-se de que o arquivo da imagem está no diretório correto.

• Verifique se o nome do arquivo foi escrito corretamente.

• Consulte as mensagens de erro no terminal para detalhes.

## Contribuições
Este projeto foi criado para fins educativos. Fique à vontade para sugerir melhorias ou reportar problemas!

**Divirta-se processando imagens!**





