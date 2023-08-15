# Template de trabalhos para Lego II

O arquivo [artigo.qmd](artigo.qmd) é um *template* de documento acadêmico usando [quarto](https://quarto.org/). Diferentemente de um arquido de *Word*, este é um arquivo de texto simples, que pode ser editado em qualquer editor de texto usando sintaxe [Markdown](https://www.markdownguide.org/basic-syntax/). Entre outras vantagens, ele nos livrará de ter de formatar documento; de inserir bibligrafia manualmente; e de ter de copiar e colar resultados de análises feitas no `R`.

## Instalação

Para usar o *template*, é necessário ter o `R` e o `quarto` instalados. Para instalar o `quarto`, busque a versão adequada para o seu computador em:

- <https://quarto.org/docs/get-started/>

Feito isso, é necessário instalar uma distribuição de [LaTeX](https://www.latex-project.org/get/). Para isso, o melhor é usar [tinytex](https://yihui.org/tinytex/). Para instalar, rode o seguinte código no `R`:

```r
install.packages("tinytex")
tinytex::install_tinytex()
```

## Uso

Para usar o *template*, basta abrir o arquivo [artigo.qmd](artigo.qmd) no [RStudio](https://rstudio.com/products/rstudio/download/), e clicar no botão `Render`. O arquivo [artigo.pdf](artigo.pdf) será gerado.

Alternativamente, também é possível compilar o arquivo do terminal digitando:

```bash
quarto render artigo.qmd
```