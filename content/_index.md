---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biographie
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Compétences
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '2'
  - block: experience
    content:
      title: Expérience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Ingénieur de recherche
          company: IMT Mines Albi - CGI
          company_url: https://cgi.imt-mines-albi.fr
          location: France - Tarn
          date_start: 2021-04-01
          date_end:
          description: >
            Projet principal: Advanced Call centers for Deaf Community

            Tâches assignés:
              * Développement d'un prototype de planification du centre d'appel Elioz / Ivès
              * Encadrement d'une thèse sur le volet gestion et analyse des données
              * Aide à la valorisation des codes de calculs développé dans le cadre du projet
              * Support numérique pour le personnel de recherche
        - title: Post-Doctorant
          company: Université Savoie Mont-Blanc - LOCIE / LAMA
          company_url: https://www.univ-smb.fr/
          location: France - Auvergne Rhone Alpes
          date_start: 2018-05-01
          date_end: 2021-04-01
          description: |
            Double projet:

            **[ANR FRAISE:](https://anr.fr/Projet-ANR-16-CE06-0011)** Films Ruisselants Absorbants à Instabilités de Surface : Exploration

            **[Projet Européen OPTIWIND - HORIZON 2020, consortium Clean Sky 2:](https://cordis.europa.eu/project/id/785300/fr)** Optimized cockpit windshield for large diameter business aircraft

            Tâches assignés:

            - Modélisation
            - Résolution numérique
            - Support numérique à la recherche
        - title: Doctorant
          company: Université Savoie Mont-Blanc - LOCIE
          company_url: https://www.univ-smb.fr/
          location: France - Auvergne Rhone Alpes
          date_start: 2014-11-01
          date_end: 2018-03-01
          description: >
            Doctorat - Optimisation d'échangeur de chaleur à films ruisselants.
    design:
      columns: '2'

  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: data
          tag: data
        - name: simulation
          tag: simulation
        - name: bio-informatique
          tag: bioinfo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

  - block: collection
    id: featured
    content:
      title: Publications principales
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation

  - block: contact
    id: contact
    content:
      title: Contact
      # Contact (add or remove contact options as necessary)
      email: contact@celliern.io
      autolink: true
    design:
      columns: '2'
---
