```mermaid
classDiagram
    Personne <|-- Citoyen
    Citoyen <|-- CitoyenActif
    Citoyen <|-- CitoyenProfessionnel
    Citoyen <|-- CitoyenIndividuel

  class Personne {
      +int age
      +String genre
      +String nom
  }

  class Citoyen {
      <<Base>>
      +String numIdentite
      +String statutJuridique
      +participerProjet()
      +voter()
  }

  class CitoyenIndividuel {
      +String situation (ex: Etudiant, Sans emploi)
      +String centresInteret
      +consulterInformation()
  }

  class CitoyenActif {
      +String association
      +exprimerAvis()
  }

  class CitoyenProfessionnel {
      +String fonction
      +agirEnFonction()
  }

  CitoyenProfessionnel <|-- CitoyenPublic
  CitoyenProfessionnel <|-- CitoyenPrive
  
```
