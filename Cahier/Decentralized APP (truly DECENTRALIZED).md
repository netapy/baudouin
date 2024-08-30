---
Created: 2020-11-02T12:51
---
- On peut connecter deux clients SANS AUCUN SERVEUR (vraiment, même pas de signaling server) à partir du moment ou on a le SDP offer (bout de texte donnant _l'adresse_ du client).  
      
    [https://jsfiddle.net/jib1/nnc13tw2/](https://jsfiddle.net/jib1/nnc13tw2/)
    
    **—> Problématique ?** Comment le communiquer facilement ? En qr code !
    
- La string SDP offer est trop grosse pour être communiquée en QR code  
      
    **MAIS**  
    Il y a un algo de compression texte UNIX  
      
    [http://www.unit-conversion.info/texttools/compress/](http://www.unit-conversion.info/texttools/compress/)
- Il suffit de compresser la SDP offer, la convertir en QR CODE, et l'afficher au client qui veut se connecter, qui va ensuite la décrypter et envoyer sa réponse au local SDP. A ce moment la on est parfaitement SERVER-LESS. [https://cozmo.github.io/jsQR/](https://cozmo.github.io/jsQR/)
  
- [x] Tester la connexion sans serveur grâce au protocol SDP (?)
- [ ] Voir si les SDP on pas des éléments qui se répètent (pour raccourcir la string potentiellement