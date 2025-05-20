This is a project presented as a poster for the conference of Una quae est omnia (?) Antike Universalreligionen im Spannungsfeld zwischen Lokalität und Überregionalität am Beispiel der Isis- und Osiris-Kulte
# Repository structure

- `LOGO_info_visualization/`  
  Figures for motif analysis using sequence logos

- `jaccard_bigrams_clustering_visualization/`  
  Cluster visualizations based on bigram Jaccard similarity

- `Poster_What Can Epithet Strings Reveal.pdf`  
  The poster

- `annotation_isis_epithets.json`  
  Structured annotations of Isis epithets in JSON format

- `epithet_heatmap.svg`  
  Heatmap revealing regional preferences of assigning epithets to Isis

- `epithet_triples_heatmap.svg`  
  Heatmap of epithet triples revealing recurring semantic modules of epithets across sites

- `legend_for_bioinfo_analysis.svg`  
  Legend for plots generated with bioinformatics techniques

  # Dataset for Isis epithets
  ## data structure
  each element inside of the JSON file is a relief block, in which the epithet strings of Isis are mentioned
  ### metadata
  including location information and scene title of the reliefs of the inscriptions and related publications
  ### layout
  giving the division of the areas and the figures mentioned in the areas in the scenes
  ### text block
  Each text block is divided into two parts of epithets and action. The block is either a block next to a figure related with Isis or a divine column referring to Isis.
  #### epithets
  {
            "e": "#sps.t wsr.t",
            "t": "venerable and powerful",
            "k": "#sps.t wsr.t",
            "kt": "Q"
          }
  
e: transliteration of epitihet

t: translation of epithet
！！！Many of the translations are directly taken or translated from the existing translations listed in Bibliogrpahy.

k: type of epithet
！！！ the standard for categorification of the types of epithets and the realted Python code will be uploaded later.

kt: motif of the type of translation

  #### action
  It should either be the verbal sentence next to the figure of Isis (and also next to the epithet strings) or the verbal sentence inside of the dvine column
  If there is no such verbal descriptions, then the fields for action is left with ∅.
  {
            "a": "dj =j n =k nswy.t n z#a =j, #hr-b#hd.tj  (I give the kingship to my son, Horus-Behdety)",
            "at": "giving kingship"
          }
  
  a: transliteration of the action
  
  at: motif of the action

  ## Bibliography
  ### Source inscriptions
  D I = Chassinat, Émile 1934. Le temple de Dendara: tome premieri. Le Caire: Imprimerie de l'Institut français d'archéologie orientale
  
  D Mammisis = Daumas, François 1959. Les mammisis de Dendara. Publications de l'Institut Français d'Archéologie Orientale. La Caire: Institut Français d'Archéologie Orientale
  
  Dendera, le Temple d'Isis = Cauville, Sylvie 2007. Dendara: le temple d'Isis, 2 vols. Kairo: Institut Français d'Archéologie Orientale
  
  DC = Zivie-Coche, Christiane 2023. Le temple de Deir Chelouit V. Temples; Chelouit 5. Le Caire: Institut Français d'Archéologie Orientale
  
  Kalabchah = Gauthier, Henri 1911-1914. Le temple de Kalabchah, 2 vols. Les temples immergés de la Nubie. Le Caire: Institut français d'archéologie orientale
  
  Philae Benedite = Bénédite, Georges 1893-1895. Le temple de Philæ. Mémoires publiés par les membres de la Mission Archéologique Française au Caire 13 (1-2). Paris: Ernest Leroux. Description et histoire de l'île de Philæ. Première partie: textes hiéroglyphiques
  
  Philae, Birth house = Kockelmann, Holger and Erich Winter 2016. Philae III: Die zweite Ostkolonnade des Tempels der Isis in Philae (CO II und CO II K), 2 vols. Mit einem Beitrag von Shafia Bedier; Zeichnungen von Dr. Otto Daum, Irmtraud Noering, Ulrike Denis und Silke Caßor-Pfeiffer. Österreichische Akademie der Wissenschaften, Denkschriften der Gesamtakademie 78. Wien: Verlag der Österreichischen Akademie der Wissenschaften
  
  
  Cauville, S. 1998. Dendara I: Traduction. Photographs by A. Lecler. Orientalia Lovaniensia Analecta 81. Leuven: Peeters
  
  Cauville, Sylvie 2009. Dendara: le temple d'Isis, 2 vols. Orientalia Lovaniensia Analecta 178-179. Leuven: Peeters

