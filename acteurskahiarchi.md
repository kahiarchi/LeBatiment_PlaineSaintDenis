```mermaid
classDiagram
    Personne <|-- Citoyen
    Citoyen <|-- CitoyenActif
    Citoyen <|-- CitoyenProfessionnel
    CitoyenProfessionnel <|-- CitoyenPublic
    CitoyenProfessionnel <|-- CitoyenPrive

  class Personne {
      +int age
      +String genre
      +String nom
  }

  class Citoyen {
      +String numIdentite
      +String communeRattachement
      +String statut (ex: Electeur, Resident)
      +boolean estInscritSurListes
      +voter(String scrutin)
      +signerPetition(String sujet)
      +consulterProjetPublic()
  }

  class CitoyenActif {
      +String association
      +String roleAsso
      +exprimerAvis()
      +proposerInitiative()
  }

  class CitoyenProfessionnel {
      +String fonction
      +String domaine
      +String siret_ou_idProf
      +agirEnFonction()
  }

  class CitoyenPublic {
      +String institution
      +String service
      +gererProjet()
  }

  class CitoyenPrive {
      +String entreprise
      +String secteur
      +realiserProjet()
  }
  
```
