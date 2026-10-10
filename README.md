# 🎓 Data Warehouse Universitário - Foco no Professor (Star Schema)

## 📖 Sobre o Projeto
Este projeto foi desenvolvido como solução para o desafio acadêmico de modelagem dimensional. O objetivo principal foi migrar uma estrutura de banco de dados relacional complexa para um modelo em estrela (**Star Schema**) utilizando o **Power BI**, com foco estrito na **análise de performance, alocação de carga horária e desempenho dos Professores**.

> ⚠️ Conforme os requisitos do desafio, os dados individuais de alunos foram omitidos e convertidos em métricas agregadas na tabela fato para garantir o foco total na análise docente.

## 📐 Estrutura do Modelo Dimensional
O modelo foi desnormalizado a partir do diagrama relacional original, resultando nas seguintes tabelas conectadas em relacionamentos de 1 para muitos (1:*):
*   **`Fato_Oferta_Academica`**: Centraliza os IDs de ligação e armazena as métricas quantitativas (`Carga_Horaria_Faturada` e `Nota_Final`).
*   **`Dim_Professor`**: Nome e nível de titulação dos docentes.
*   **`Dim_Departamento`**: Mapeamento de setores, campi e seus respectivos coordenadores.
*   **`Dim_Disciplina`**: Cadastro de disciplinas com quebra de carga horária teórica/prática.
*   **`Dim_Curso`**: Graduações e modalidades de ensino (Presencial/EAD).
*   **`Dim_Data`**: Dimensão calendário criada para fornecer inteligência de tempo e análise de ofertas por ano e semestre.

## 🛠️ Tecnologias Utilizadas
*   **Power BI:** ETL (Power Query), modelagem de dados e construção do painel visual.
*   **Modelagem Dimensional:** Conceitos Kimball (Tabelas Fato, Dimensões e Surrogate Keys).
*   
## 👨‍💻 Autor
Desenvolvido por Gabriela Pereira das Neves no âmbito da jornada de transição e especialização em Dados e Tecnologia.
