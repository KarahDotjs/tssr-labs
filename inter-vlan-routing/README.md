#  Lab — Inter-VLAN Routing (Router-on-a-Stick)

## 🎯 Contexte & Objectif

Dans ce lab, j'ai configuré un réseau d'entreprise composé de deux VLANs distincts — **VLAN 10 IT** et **VLAN 20 COMPTA** — sur un switch Cisco 2960 connecté à un routeur Cisco 2911.

L'objectif était de **segmenter le réseau** en isolant les deux départements dans des VLANs séparés, puis de les faire **communiquer entre eux** grâce à une technique appelée **Router-on-a-Stick**.

Sans cette configuration, PC0 et PC1 seraient invisibles l'un pour l'autre malgré le fait d'être sur le même switch physique. Grâce au trunk et aux sous-interfaces du routeur, les trames peuvent traverser les VLANs de manière contrôlée et sécurisée.

**Ce lab couvre les compétences suivantes :**
- Création et nommage de VLANs
- Affectation de ports en mode access
- Configuration d'un lien trunk 802.1Q
- Routage inter-VLAN via sous-interfaces (Router-on-a-Stick)
- Plan d'adressage IP et configuration des passerelles
