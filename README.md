# Analisador de Ligacoes Quebradas e Erros 404

[![Analisador Ligacoes Quebradas](https://img.shields.io/badge/TAVARDT-Broken%20Links-5b3cf5.svg)](https://tools.tavardt.com/pt/analisador-ligacoes-quebradas/)
[![Jurisdicao](https://img.shields.io/badge/Jurisdicao-Portugal-00C853.svg)](https://ag.tavardt.com/pt/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Detecao de ligacoes mortas, inspecao de codigos de resposta HTTP e preservacao do crawl budget.

Desenvolvido e mantido pela equipa de infraestrutura web da **[TAVARDT Portugal](https://ag.tavardt.com/pt/)**.

---

## Capacidades de Inspecao de Ligacoes Quebradas

* **Auditoria de Hiperligacoes**: Analise sistematica de todas as ligacoes internas e externas contidas no documento HTML.
* **Detecao de Erros HTTP 404 e 500**: Diagnostico de respostas com falha de cliente ou servidor que interrompem a navegacao.
* **Protecao de Orcamento de Rastreio (Crawl Budget)**: Eliminacao de ligacoes mortas que prejudicam a eficiencia dos motores de busca.
* **Verificacao de Textos Ancoras**: Inspecao de descricoes de ligacao para garantia de acessibilidade e contexto semantico.
* **Metrica de Integridade de Ligacoes**: Classificacao de 0 a 100 com detalhe de ligacoes inoperacionais.

---

## Instalacao e Execucao

Requer Python 3.8 ou superior recorrendo apenas a modulos standard.

```bash
git clone https://github.com/TAVARDT-Portugal/broken-links-checker-pt.git
cd broken-links-checker-pt
python broken_links_scanner.py https://empresa.pt
```

Modo de saida estruturada JSON:

```bash
python broken_links_scanner.py https://empresa.pt --json
```

---

## Ferramenta Oficial na Web

Efetue analises completas na plataforma online:

* **[Analisador de Ligacoes Quebradas Oficial](https://tools.tavardt.com/pt/analisador-ligacoes-quebradas/)**
* **[Portal TAVARDT Portugal](https://ag.tavardt.com/pt/)**

---

## Consultoria Especializada

Para modernizacao de ligacoes internas segundo Normas Europeias de Integridade Web e W3C, contacte a **[TAVARDT Portugal](https://ag.tavardt.com/pt/contato/)**.
