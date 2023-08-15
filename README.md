# Template de trabalhos para Lego II

O arquivo [artigo.qmd](artigo.qmd) é um *template* de documento acadêmico usando [quarto](https://quarto.org/). Diferentemente de um arquivo de *Word*,este pode ser editado em qualquer editor de texto usando [Markdown](https://www.markdownguide.org/basic-syntax/). Entre outras vantagens, ele dispensa termos de formatar o documento final; de inserir bibligrafia manualmente; e de ter de copiar e colar resultados de análises feitas no `R`.

## Instalação

Para usar o *template*, é necessário ter o `R` e o `quarto` instalados. Para instalar especificamente o `quarto`, busque a versão adequada para o seu computador em:

- <https://quarto.org/docs/get-started/>

Feito isso, é necessário instalar uma distribuição de [LaTeX](https://www.latex-project.org/get/). Para isso, o melhor é usar [tinytex](https://yihui.org/tinytex/) rodando o seguinte código no `R`:

```r
install.packages("tinytex")
tinytex::install_tinytex()
```

Finalmente, instale o pacote `quarto` para `R` com:

```r
install.packages("quarto")
```

## Uso

Com as dependências anteriores instaladas, para usar o *template* basta abrir o arquivo [artigo.qmd](artigo.qmd) no [RStudio](https://rstudio.com/products/rstudio/download/), editar seu conteúdo como quiser e clicar no botão `Render`. O arquivo [artigo.pdf](artigo.pdf) será gerado.

Também é possível compilar o arquivo executando o seguinte código em `R`:
    
```r
quarto::render("artigo.qmd")
```

Ou, alternativamente, executando no terminal:

```bash
quarto render artigo.qmd
```

