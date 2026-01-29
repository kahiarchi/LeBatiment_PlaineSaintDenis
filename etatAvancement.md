```mermaid
gantt
    dateFormat  2026-01-29

    title      Participation citoyenne dans les projets urbains au sein du quartier de La Plaine Saint-Denis


 %% Styles
    classDef doneTask fill:#2ecc71,color:#ffffff,stroke:#1e8449,stroke-width:1px
    classDef activeTask fill:#3498db,color:#ffffff,stroke:#21618c,stroke-width:1px
    classDef futureTask fill:#f39c12,color:#ffffff,stroke:#b9770e,stroke-width:1px
    classDef milestoneTask fill:#e74c3c,color:#ffffff,stroke:#922b21,stroke-width:2px


    section Cadrage du projet
    Définition du sujet et objectifs        :done, t1, 2025-09-15, 2025-09-22
    Formulation de la problématique         :done, t2, 2025-09-22, 2025-09-29
    class t1,t2 doneTask

    section Veille documentaire et numérique
    Recherche documentaire (web, articles) :done, t3, 2025-09-22, 2025-10-10
    Mise en place RSS, alertes, Sindup      :done, t4, 2025-09-25, 2025-10-15
    class t3,t4 doneTask

    section Définition du terrain
    Analyse historique et urbaine           :done, t5, 2025-10-01, 2025-10-15
    Identification des acteurs              :done, t6, 2025-10-10, 2025-10-20
    class t5,t6 doneTask

    section Conception de l’enquête
    Élaboration du questionnaire            :done, t7, 2025-10-15, 2025-11-05
    Paramétrage LimeSurvey                  :done, t8, 2025-11-01, 2025-11-10
    class t7,t8 doneTask

    section Ajustements pédagogiques
    Corrections questionnaire – V1          :done, t9, 2025-11-10, 2025-11-25
    Corrections questionnaire – V2          :done, t10, 2025-12-01, 2025-12-07
    Corrections questionnaire – V3          :done, t11, 2025-12-07, 2025-12-10
    class t9,t10,t11 doneTask

    section Diffusion du questionnaire
    Diffusion en ligne                      :active, t12, 2025-12-10, 2026-01-31
    Diffusion terrain (flyers, rue)         :active, t13, 2025-12-15, 2026-01-31
    class t12,t13 activeTask

    section Entretiens terrain
    Conception des grilles d’entretien      :done, t14, 2025-11-25, 2025-12-05
    Réalisation des entretiens              :active, t15, 2025-12-10, 2026-02-15
    class t14 doneTask
    class t15 activeTask

    section Analyse des données
    Analyse des questionnaires              :t16, 2026-01-20, 2026-02-20
    Analyse qualitative des entretiens      :t17, after t15, 20d
    class t16,t17 futureTask

    section Rédaction et restitution
    Rédaction analyse et discussion         :t18, 2026-02-15, 2026-03-10
    Finalisation du rapport                 :t19, 2026-03-01, 2026-03-20
    Présentation finale                     :milestone, t20, 2026-03-20, 0d
    class t18,t19 futureTask
    class t20 milestoneTask
```
