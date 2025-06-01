
# 📈 Web Scraper de Fundos Imobiliários (ClubeFII)

Este projeto é um scraper simples que coleta informações de fundos imobiliários (FIIs) do site [Clube FII](https://www.clubefii.com.br/) e exporta os dados para um arquivo CSV. A extração é feita com `Selenium`, `BeautifulSoup` e `pandas`.

---

## 🔧 Tecnologias Utilizadas

* Python 3.x
* Selenium
* BeautifulSoup (bs4)
* pandas
* Firefox + Geckodriver

---

## 📦 Instalação

1. Clone este repositório:

   ```bash
   https://github.com/vinicius7m/web-scrapper-fiis.git
   ```

2. Crie um ambiente com o Conda e instale as dependências:

   ```bash
   conda env create -f environment.yml
    conda activate fii-scraper

   ```

3. Certifique-se de ter o [Firefox](https://www.mozilla.org/pt-BR/firefox/new/) instalado e o [Geckodriver](https://github.com/mozilla/geckodriver/releases) disponível no seu PATH.

---

## ▶️ Como usar

Execute o script principal:

```bash
python scraper_fii.py
```

O script irá:

1. Acessar a página de um FII no ClubeFII.
2. Aguardar o carregamento completo da tabela de dados.
3. Extrair os dados da tabela principal (`id="tabela_profile"`).
4. Exibir colunas específicas no terminal.
5. Exportar todos os dados da tabela para um arquivo `fundos_imobiliarios.csv`.

---

## 🧪 Exemplo de saída (colunas extraídas)

```
Administrador | Código Negociação | Cotação | Valor Último Rendimento | Yield de Distribuição 1 Mês
```

---

## 📁 Arquivo Gerado

* `fundos_imobiliarios.csv`: contém os dados estruturados dos fundos, prontos para análise.

---

## 🚧 Melhorias Futuras

* Geração de gráficos com `matplotlib`.

---

## 📄 Licença

Este projeto está sob a licença MIT.