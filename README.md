# PAXOS
# Messenger.py
La classe Messenger encapsule la stratégie de transmission de message pour l'application. Les instances BaseReplicatedValue envoient des messages en appelant l'une des méthodes send_ <message-type> du Messagerie et reçoivent des messages en spécifiant une méthode receive_ <message-type> pour chaque type de message qu'elle prend en charge. La classe messager recherchera dynamiquement la méthode de traitement des paquets entrants en recherchant la hiérarchie des classes pour une méthode appropriée nommée basée sur le type de message du message entrant.

Pour garder les choses simples pour cet exemple, les messages sont envoyés par UDP et utilisent un format de codage JSON simple.
