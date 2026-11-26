<p align="center">
  <a href="https://ag.tavardt.com/pt/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="1024" />
  </a>
</p>

# Analisador de Ligações Quebradas e Erros 404

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Analisador Ligações Quebradas](https://img.shields.io/badge/TAVARDT-Broken%20Links-5b3cf5.svg)](https://tools.tavardt.com/pt/analisador-ligações-quebradas/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Auditoria de hiperligacoes internas e externas, identificacao de erros HTTP 404, ligacoes inativas e preservacao do crawl budget.

***

## Vetores de Risco e Impacto Operacional nas Ligacoes Web

Ligacoes quebradas com codigos de erro HTTP 404 e 500 frustram os utilizadores e dissipam o orcamento de rastreio dos motores de busca em Portugal. Os robots de indexacao abandonam o varrimento ao encontrar becos sem saida, prejudicando a atualizacao do catalogo.

Hiperligacoes externas corrompidas enfraquecem a autoridade do dominio e prejudicam a citacao em respostas geradas por IA. A auditoria continua protege a distribuicao interna de PageRank e assegura percursos fluidos de navegacao.

***

## Capacidades Centrais de Auditoria Tecnica

* **Extracao e Normalizacao de Ligacoes**: Analisa elementos href descartando referencias locais, chamadas telefonicas e enderecos de correio eletronico.
* **Segregacao de Hiperligacoes Internas e Externas**: Distingue de forma automatica as URLs internas da organizacao em relacao a destinos externos.
* **Sondagem Otimizada via Metodo HEAD**: Inspeciona codigos de estado sem transferir o conteudo para poupar largura de banda de rede.
* **Mecanismo de Recurso com Metodo GET**: Repete o pedido em GET caso o servidor remoto bloqueie o metodo HEAD com status 403 ou 405.
* **Identificacao de Erros HTTP e Quebras de Sessao**: Cataloga anomalias 4xx, 5xx e falhas de resolucao com diagnostico detalhado.
* **Indice de Qualidade de Ligacoes**: Atribui uma pontuacao tecnica de 0 a 100 categorizada em SATISFACTORY, ADVISORY ou UNSATISFACTORY.
* **Exportacao Estruturada em Formato JSON**: Facilita a integracao com esteiras de desenvolvimento atraves de opcoes rapidas de linha de comando.

***

## Instalacao e Execucao

Requer Python 3.8 ou superior utilizando exclusivamente bibliotecas padrao.

```bash
git clone https://github.com/TAVARDT-Portugal/broken-links-checker-pt.git
cd broken-links-checker-pt
python broken_links_scanner.py https://empresa.pt
```

Para gerar a saida em formato estruturado JSON em esteiras de integracao continua:

```bash
python broken_links_scanner.py https://empresa.pt -j
```

***

## Perguntas Frequentes (FAQ Tecnico)

### 1. Como erros HTTP 404 e links mortos prejudicam o orcamento de rastreamento?
Os motores de busca dedicam uma cota finita de requisicoes para explorar cada dominio. Encontrar links quebrados consome essa capacidade em rotas inexistentes, atrasando a indexacao de conteudos novos ou atualizados.

### 2. Por que o validador utiliza requisicoes HTTP HEAD com reintento em GET?
A ferramenta realiza a checagem inicial via HEAD para avaliar codigos HTTP sem baixar o corpo da pagina. Caso o servidor de destino bloqueie o metodo HEAD com status 403 ou 405, o script efetua nova tentativa em GET para eliminar falsos positivos.

### 3. De que maneira links internos quebrados dissipam a distribuicao de PageRank?
Os links internos atuam como canais primarios para transmitir autoridade e contexto tematico atraves da hierarquia do site. Rotas quebradas interrompem esse fluxo prematuramente, deixando subpaginas orfas e prejudicando o ranqueamento organico.

### 4. Quais os riscos operacionais de manter links externos corrompidos no conteudo?
Apontar para dominios externos desativados ou redirecionados expoe os visitantes a riscos de seguranca e compromete a reputacao institucional. Sistemas modernos de busca e IA avaliam a integridade das referencias, penalizando paginas com fontes inoperantes.

### 5. Por que a auditoria continua de links e fundamental apos migracoes de site?
Projetos de migracao e reestruturacao de URLs geram rotas quebradas com frequencia quando regras de redirecionamento falham. A inspecao automatizada identifica falhas 4xx e 5xx imediatamente, protegendo a autoridade de busca antes de quedas de trafego.

***

## Consultoria em Arquitetura de Ligacoes e Eficiencia de Indexacao

Para portais de grande dimensao e alinhamento com as diretrizes W3C e padroes de pesquisa, consulte a equipa da **TAVARDT**.

***

## Links Uteis

* **Portal Corporativo:** https://ag.tavardt.com/pt/
* **Suite de Diagnosticos:** https://tools.tavardt.com/pt/
* **Contacto Tecnico:** https://ag.tavardt.com/pt/contacto/

***

### Licenca
Distribuido sob a Licenca MIT. Consulte o arquivo LICENSE para termos completos.

***

© 2026 TAVARDT. Todos os direitos reservados.
