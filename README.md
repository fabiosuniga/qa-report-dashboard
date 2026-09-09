<img width="1251" height="697" alt="image" src="https://github.com/user-attachments/assets/db363872-cc43-4067-82f1-2a33cde557ad" /><p align="center">
  <img src="header-qa-readme.png" alt="Header Painel Interativo de QA" width="100%">
</p>

# Painel Interativo de QA (QA Report Dashboard)

> Painel analítico 100% **client-side** (sem dependência de banco de dados ou backend), projetado para auditoria ágil, validação de critérios de aceite e controle de qualidade contínuo em sistemas e fluxos de software.
---

### Visão Geral

![Visão Geral do Painel](<img width="1251" height="697" alt="tela-inicial" src="https://github.com/user-attachments/assets/0ecbad5c-3bb5-4317-bce1-4cfcce2dd0e3" />
)

# Painel Interativo de QA (QA Report Dashboard)

> Painel analítico 100% **client-side** (sem dependência de banco de dados ou backend), projetado para auditoria, validação de prompts e controle de qualidade contínuo em sistemas de IA e Chatbots.

---

### O Problema

A validação manual de respostas de modelos de linguagem frequentemente depende de planilhas extensas ou arquivos de texto sem padronização. 

Este projeto consolida o processo de auditoria em uma interface visual focada em produtividade, permitindo avaliar lado a lado:
* **Prompt original**
* **Resposta obtida pelo modelo**
* **Gabarito / Resposta de referência**

Gera indicadores automáticos de conformidade e relatórios prontos para distribuição executiva.

---

### Principais Recursos

* **Métricas em Tempo Real:** Consolidação automática da taxa de acurácia com base nas classificações (*Correta*, *Imprecisa*, *Incorreta* e *Erro*).
* **Gestão Ágil de Casos:** Criação, duplicação e exclusão rápida de cartões de avaliação.
* **Filtros Segmentados:** Isolamento dinâmico de cards por status crítico (ex.: exibição exclusiva de falhas).
* **Exportação Otimizada para PDF:** Reestruturação de layout via CSS paged media/canvas para entrega sem quebras indesejadas de blocos.
* **Portabilidade em Arquivo Único (HTML):** Exportação do estado da sessão em um único arquivo `.html` autossuficiente, preservando total interatividade offline para outros revisores.
* **Suporte PWA:** Instalação nativa em desktop e mobile com funcionamento resiliente via cache.
* **Sanitização de Entrada:** Limpeza automática do clipboard ao colar dados com <kbd>Ctrl</kbd> + <kbd>V</kbd>, prevenindo ruídos de formatação externa.

---

### Demonstração e Uso

Acesse a aplicação pronta para uso via GitHub Pages:  
**[Acessar Live Demo](https://fabiosuniga.github.io/qa-report-dashboard/)**

#### Fluxo de Trabalho

1. **Entrada:** Crie um novo cartão ou duplique um registro de teste existente.
2. **Dados:** Insira a instrução enviada (*prompt*), o retorno da IA e o resultado esperado.
3. **Auditoria:** Selecione o status de validação no seletor correspondente.
4. **Relatório:** Clique em **Exportar PDF** ou salve a versão estática navegável para compartilhamento.

![Demonstração da Exportação em PDF](<img width="1921" height="837" alt="tela-inicial-pdf" src="https://github.com/user-attachments/assets/295136d4-85ec-47c6-b3fd-f4bbe3dcca69" />
)

---

### Stack Tecnológica

| Camada | Tecnologia | Aplicação |
| :--- | :--- | :--- |
| **Interface** | HTML5 / CSS3 Moderno | Custom Properties (CSS variables), Grid e Flexbox |
| **Lógica** | JavaScript (Vanilla) | Manipulação direta de DOM e gerenciamento de estado |
| **Offline** | Service Workers (PWA) | Cache inteligente e suporte à instalação do app |
| **Impressão** | html2pdf.js | Conversão client-side de elementos DOM para documento PDF |

---
