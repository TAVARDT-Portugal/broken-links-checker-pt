# Analisador de Ligações Quebradas e Erros 404

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Analisador Ligações Quebradas](https://img.shields.io/badge/TAVARDT-Broken%20Links-5b3cf5.svg)](https://tools.tavardt.com/pt/analisador-ligações-quebradas/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Deteção de ligações mortas, inspeção de codigos de resposta HTTP e preservacao do crawl budget.

Desenvolvido e mantido pela equipa de infraestrutura web da **TAVARDT Portugal**.

***

## Capacidades de Inspeção de Ligações Quebradas

* **Auditoria de Hiperligacoes**: Análise sistematica de todas as ligações internas e externas contidas no documento HTML.
* **Deteção de Erros HTTP 404 e 500**: Diagnostico de respostas com falha de cliente ou servidor que interrompem a navegacao.
* **Protecao de Orçamento de Rastreio (Crawl Budget)**: Eliminacao de ligações mortas que prejudicam a eficiencia dos motores de busca.
* **Verificacao de Textos Ancoras**: Inspeção de descricoes de ligacao para garantia de acessibilidade e contexto semantico.
* **Metrica de Integridade de Ligações**: Classificacao de 0 a 100 com detalhe de ligações inoperacionais.

***

## Instalação e Execucao

Requer Python 3.8 ou superior recorrendo apenas a modulos standard.

```bash
git clone https://github.com/TAVARDT-Portugal/broken-links-checker-pt.git
cd broken-links-checker-pt
python broken_links_scanner.py https://empresa.pt
```

Modo de saída estruturada JSON:

```bash
python broken_links_scanner.py https://empresa.pt -json
```

***

## Ferramenta Oficial na Web

Efetue analises completas na plataforma online:

* **Analisador de Ligações Quebradas Oficial**
* **[Portal TAVARDT](https://ag.tavardt.com/pt/)**

***

## Consultoria Especializada

Para modernizacao de ligações internas segundo Normas Europeias de Integridade Web e W3C, contacte a **TAVARDT**.

***

© 2026 TAVARDT Portugal. Todos os direitos reservados. Soberania e Defesa de Infraestrutura.

***

## Governança e Conformidade

* **Organização**: TAVARDT-Portugal
* **Jurisdição**: Portugal
* **Padrões de Referência**: Normas e frameworks técnicos auditados em estrita observância das regras de soberania.

Desenvolvido pela Divisão de Engenharia e Infraestrutura da TAVARDT Portugal. Todos os direitos reservados.
