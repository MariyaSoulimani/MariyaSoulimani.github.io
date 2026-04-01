---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

design:
  # Default section spacing
  spacing: '0'

sections:
  # AJOUTER LES PROJETS DE ROUMAYSSA ICI — contenu : dossier content/projects/ (voir aussi content/projects/_index.md)
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Bonjour, je suis"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "Je me passionne pour"
        strings:
          - "la gestion et l'administration des affaires"
          - "l'entrepreneuriat"
          - "la création de contenu"
          - "les défis qui forgent une carrière solide"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: Voir mes projets
          url: "#projects"
          icon: arrow-down
        - text: Me contacter
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]
  
  - block: portfolio
    id: projects
    content:
      title: "Projets & Expériences"
      subtitle: "Mes réalisations et expériences professionnelles"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: Tous
          tag: '*'
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  - block: tech-stack
    id: skills
    content:
      title: "Compétences"
      subtitle: "Savoir-faire et outils"
      categories:
        - name: Compétences humaines
          items:
            - name: Travail en équipe
              icon: heroicons/outline/user-group
            - name: Créativité et esprit d'initiative
              icon: heroicons/outline/sparkles
            - name: Leadership inspirant
              icon: heroicons/outline/flag
        - name: Outils et numériques
          items:
            - name: Maîtrise de Word, PowerPoint, Canva
              icon: heroicons/outline/document-text
            - name: Notions de base en intelligence artificielle
              icon: heroicons/outline/cpu-chip
            - name: Édition de contenu avec CapCut
              icon: heroicons/outline/film
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # SECTION À COMPLÉTER : expérience professionnelle (bloc resume-experience retiré faute de poste à afficher)
  
  - block: contact-info
    id: contact
    content:
      title: Me contacter
      subtitle: "Échanges, stage ou collaborations"
      text: |-
        Je suis basée à Meknès, Maroc. Vous pouvez m'écrire ou m'appeler pour discuter d'un stage ou de toute opportunité en lien avec la gestion et l'administration des affaires.
      email: romayssaebenahmed@gmail.com
      phone: "+212 644-692238"
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  - block: cta-card
    content:
      title: "Ouverte aux opportunités de stage"
      text: |-
        **Étudiante en gestion** à la recherche d'un stage pour mettre en pratique mes connaissances, découvrir le fonctionnement d'une entreprise et contribuer avec sérieux aux missions confiées.
        
        Vous pouvez télécharger mon CV ci-dessous.
      button:
        text: 'Télécharger mon CV'
        url: uploads/resume.pdf
        new_tab: true
    design:
      card:
        # Light mode: soft pastel theme gradient | Dark mode: rich deep gradient
        css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
        text_color: dark
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
