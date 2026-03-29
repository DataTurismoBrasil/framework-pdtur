```mermaid
flowchart LR

%% =====================
%% BASE
%% =====================

subgraph F1["BASE DO PDTUR"]
A1[Normativas e Políticas Públicas\nMTur, Estado, ODS]
A2[Documentos Orientadores\nReferenciais Técnicos]
end

%% =====================
%% ESTRUTURA DO PLANO
%% =====================

subgraph F2["ESTRUTURA DO PLANO"]
B1[Caracterização do Município]
B2[Organização do Plano\n(Subseções do PDTUR)]
end

%% =====================
%% DIAGNÓSTICO
%% =====================

subgraph F3["DIAGNÓSTICO DO TURISMO"]
C1[Oferta Turística]
C2[Demanda Turística]
C3[Infraestrutura]
C4[Governança]
C5[Dados e Informações]
end

%% =====================
%% PROGNÓSTICO
%% =====================

subgraph F4["PROGNÓSTICO"]
D1[Análise Estratégica]
D2[Definição de Diretrizes]
D3[Prioridades do Turismo]
end

%% =====================
%% PLANO DE AÇÃO
%% =====================

subgraph F5["PLANO DE AÇÃO"]
E1[Matriz de Implementação do PDTUR]
E2[Programas e Projetos]
E3[Ações, Responsáveis, Prazos]
end

%% =====================
%% MONITORAMENTO
%% =====================

subgraph F6["GESTÃO E MONITORAMENTO"]
F1A[Acompanhamento]
F2A[Avaliação]
F3A[Revisão do Plano]
end

%% =====================
%% FLUXO
%% =====================

A1 --> A2 --> B1 --> B2 --> C1
C1 --> C2 --> C3 --> C4 --> C5
C5 --> D1 --> D2 --> D3
D3 --> E1 --> E2 --> E3
E3 --> F1A --> F2A --> F3A

%% LOOP
F3A --> D1

%% =====================
%% DIMENSÕES
%% =====================

G[Governança]
H[Planejamento Estratégico]
I[Mensuração]
J[Competitividade]
K[Sustentabilidade\nTransversal]

G --- C4
G --- F1A

H --- D1
H --- D2

I --- F1A
I --- F2A

J --- F2A

K --- A1
K --- B1
K --- C1
K --- D1
K --- E1
K --- F2A
```
