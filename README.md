# Nuit du Hack 16 - Social Engineering Challenge

Ce write-up décrit la deuxième phase du challenge, celle de Social Engineering proprement dite, où SundayParan0ids a terminé à la première place.
Pour la première phase - celle de OSINT, nous vous renvoyons au write-ups des équipes arrivées dans le Top 3, autant ne regarder que ce qui est de kalitay !
Celui de Jhack Chirhack est dispo ici : https://inshallhack.org/jhack-chirhack-step-1.pdf

## Phase I: Opération Séduction

Nous avons une liste de personnes à nous mettre dans la poche afin de récupérer un maximum d'informations, si possible compromettantes. SupremIoT cherche à faire de l'évasion et du blanchiment ? Nous serons donc la Monaco Investment Bank, spécialisée dans l'optimisation, et cherchant à diversifier ses offres en y incluant des cryptomonnaies.


![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)   
The blockchain defenders !

Monaco Investment Bank, c'est:

* **Bill Laporte**, CEO, chemise hawaienne, adepte de cigares et de soirées arrosées. Cible principale: Advei Tretiakov. Approche: leur nombreux points communs.
* **Eddie Dacier**, Lead Dev, en ayant marre de MiB et cherchant à se faire débaucher. Cible principale: Umberto Ferreira. Approche: critiquer ses collègues pour récupérer des témoignages similaires, demander un job pour récupérer des infos internes.
* **Guillaume Lelouch**, 'spécialiste' de la blockchain et des cryptomonnaies. Cibles principales: Ian Kudryashov, May Chi. Approche: parler manga et magic: the gathering.
* **Volkmar**, responsable commercial. Cible principale: Benoit Rochat. Approche: money money money !

On est au clair sur l'approche, reste à la mettre en oeuvre. On se rend rapidement compte qu'il est beaucoup plus efficace de travailler en binôme ou en groupe, ce qui donnera lieu à quelques intéractions clé.

**Umberto**: Première approche en groupe, on se présente à Umberto et Benoit en tant que MiB. On demande à voir le boss (qui n'est pas encore arrivé), on sympathise. Guillaume parle fort et passe pour un parfait crétin en montrant ses bitcoins en métal achetés 3000 Eur chacun 'alors qu'un bitcoin ça en vaut 6000 ! J'ai fait l'affaire du siècle.'
La méfiance de nos interlocuteurs s'endort, ils nous prennent pour de joyeux drilles et ont presque pitié pour Bill et Eddie d'avoir à supporter Guillaume tous les jours.
Volkmar repère discrètement quelques documents intéressants au comptoir de SupremIoT, notamment sur les iles vierges.

**Advei**: Nous prenons possession d'une table et d'un sofa à l'écart. On pose les ordis, sur des pages de finances, on y laisse traîner un Nice Matin récupéré dans l'avion, une petite feuille avec marqué Monaco Investment Bank, et nous voilà avec des locaux dignes de ce nom. Bill invite Advei à venir parler business tranquillement. Pendant qu'ils parlent, notre caméra espion filme le tout. Advei commence à se détendre: nous sommes après tout sur la même longueur d'ondes lorsque l'on parle de blanchi... d'optimisation fiscale. Nous cherchons à vérifier si nous avons des clients en commun. Advei hésite, mais en lui garantissant que nous ne diront pas que les infos viennent de lui, il se met à parler. Nous apprenons que leur solution a été pentestée par Digital Security. Alors qu'il nous fait signer un document, nous en profitons pour photographier discrètement le reste de son dossier resté sur la table. Bill parle de marché chinois pour mettre l'accent sur les activités de May, mais Advei dit qu'il se méfie de la Chine. Cette info nous sera bien utile plus tard !


![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)   
 Confidence pour confidence (c’est moi que j’aime à travers vous)

**Spy VS Spy**: tout contents de notre collecte d'infos, nous commençons à débriefer un peu bruyamment... quand nous réalisons soudain qu'une autre équipe semble nous écouter à grande distance ! Décidément, même au sein de notre banque d'investissement nous n'avons pas un tel budget matériel ;)
Nous serons plus discrets désormais.

**Pickpocket en herbe**: Advei faisant des aller-retour de la chambre secrète au stand, nous avons profité du Street Fighter II arcade situé juste en face de cette chambre afin d’épier ses moindres faits et gestes. À un moment, Guillaume constate un papier dépasser de la poche d’Advei. Sans réfléchir, Eddie part à sa poursuite et profite d’un regroupement de personnes bloquant le parcours de la cible afin de lui dérober discrètement le papier contenant le QR code de la clef secrète de son wallet, le plus naturellement du monde.
 
**Digital Security**: nous pensons avoir identifié l'agent en question, qui parle régulièrement aux membres de l'équipe SupremIoT. Mais notre demande discrète d'infos sur le pentest reste vaine. (nous avons également SE quelques types qui ne jouaient pas et qui ont dû se demander pourquoi des types dans la finance étaient à la NDH :) )

**May**: Nous la voyons enfin au stand de SupremIoT ! Eddie vient taper la discute. Elle ne semble pas très réceptive, mais Eddie tient à lui laisser une carte de visite. Il fait alors tomber 'sans le faire exprès' quelques cartes Magic. Guillaume bondit: quel scandale ! Ces cartes valent hyper cher ! Eddie cherche à lui voler c'est sûr. Il enchaîne alors: mais ce tatouage, c'est un lotus noir ! Tu joues à Magic ?


![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)   
Et là, il joue une boule de feu alors qu’il n’a pas de mana rouge ! La criiise !

Alors que May acquiesce, Guillaume s'installe alors au bureau de SupremIoT et commence à lui montrer quelques cartes dont il est fier, ce qui laisse toute latitude à Bill et Volkmar pour subtiliser les QR-Codes qui se trouvent sur le bureau. Guillaume finit par prendre congé, il se sent maintenant comme chez lui chez SupremIoT.

**Ian**: Guillaume aura beau siffloter le générique de Sword Art Online durant des heures et se présenter comme Guillaume Lelouch - comme le personnage de Code Geass, clin d'oeil clin d'oeil, Ian reste insensible. Nous n'en retireront qu'une adresse email que nous avions déjà.

**Les QR-Codes**: quelle joie d'avoir récupéré ces morceaux de papier au logo de SupremIoT ! Après avoir donné notre email dans le formulaire associé, Volkmar réalise que le lien est avec Zataz.com. Après vérification, il se trouve qu'il s'agit d'une fausse piste. Nous nous sommes faits avoir comme des débutants ! Nous restons sur nos gardes vis à vis de notre boîte email. Si un mail de phishing pointe son nez, nous sommes prêts à balancer de fausses infos !


![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)   
Trop bieeeeen ! (en fait, non)

**Katrien**: la fille de Fit Bit and Strong est présente elle aussi. Guillaume lui amène Volkmar par la main, disant qu'il est trop timide pour l'approcher directement et lui demandant si elle a des conseils fitness pour lui. Lui demandant ce qu'elle fait là, nous aurons confirmation qu'elle travaille chez SupremIoT. Guillaume se demande bien pourquoi la célèbre Katrien s'abaisse à un tel boulot et finit par lui faire dire qu'elle déteste Umberto, mais c'est à peu près tout ce que nous obtiendrons. (full disclosure: on ne s'attendait pas à la trouver à la NDH, du coup on est allés la voir sans trop d'idée en tête. Bilan des courses: toujours prévoir à l'avance ce qu'on veut récupérer comme info, sinon on pédale dans la semoule !)

Nous cherchons à creuser un peu plus du côté de Digital Security mais nous resterons dans une impasse.

## Phase II: Opération Filature

Les choses se corsent: nous devons filer Advei ET Benoit, à 15h précises. Il est temps de nous séparer en deux binômes.


![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)   
OSS-117, à côté de ça, c’est du pipi de chat !

**Advei: nous devons récupérer tout son argent par n'importe quel moyen.**

15h05, personne en vue. Guillaume demande à May où est le patron, que c'est une honte, il lui a donné rendez-vous à 15h pile et il est en retard ! May s'apprête à se renseigner quand Advei nous passe devant et disparait. Guillaume se poste de nouveau à la borne d'arcade, surveillant la sortie du CEO. Mais il tombe dans un piège horrible: il se concentre trop sur le jeu vidéo et laisse passer sa cible !
Mais heureusement, Bill l'a repéré. Guillaume retrouve Bill qui observe Advei en train de parler à un type costaud identifié plus tôt sous le nom de 'M Bitcoin'. M Bitcoin a une valise menottée au poignet, et part faire un tour avec Advei.
Bill les suit pendant que Guillaume les prend à revers, prenant quelques photos de l'échange de malette au passage.
Une fois M Bitcoin parti, Guillaume se dirige franchement vers Advei, l'air affolé (et prenant de vitesse d'autres agents semblant hésitants sur la posture à adopter).
Il s'adresse à Advei comme s'ils étaient potes depuis la nuit des temps: 'Ah Advei, enfin je te retrouve ! C'est la catastrophe, des hackers chinois ont décidé de faire la peau à SupremIoT ! Tu as peut-être encore de transférer tes actifs chez nous le temps que ça se calme !'
Bill me rejoint alors, téléphone à l'oreille. 'Notre branche en Chine', explique t'il. 'Ils essaient de ralentir l'attaque mais ils ne vont pas tenir longtemps !'
Guillaume ouvre la page des comptes de Monaco Investment Bank, et le QR-Code qui permet un transfert immédiat. Advei s'execute avec son portable, et nous remercie de l'avoir tiré de ce mauvais pas. Il nous offre même 10 Bitcoins pour services rendus, ce qui nous permet de voir (et de photographier) ce que contient la malette ainsi que sa combinaison :)
Nous rassurons Advei, lui disant qu'il a fait ce qu'il faut, et que dans quelques années nous rirons de cette anecdote. Nous lui donnons rendez-vous le soir même pour faire la fête. Nous prenons également son numéro de téléphone pour le tenir au courant :p


![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)   
Y’a pas que des bitcoins là-dedans…

**Benoit: nous devons le faire avouer qu'il cherche à détourner l'argent de SupremIoT.**

Eddie et Volkmar prennent Benoit en filature, qui traine en longueur, caméra espion activée. Au bout d'un temps infini, Benoit jette un papier à la poubelle. C'est ce que nous attendions. Eddie récupère le papier, clair sur un transfert à venir et contenant un digicode (qui se révèlera le digicode du coffre de la phase d'intrusion physique ;))
Eddie prend alors Benoit à partie et lui mets la pression, menaçant de rendre l'affaire publique. Benoit préfère nier alors que les preuves matérielles et vidéo sont contre lui. Inutile d'insister.
Eddie nous mets au courant. Nous décidons alors de partir sur une autre approche: Bill va approcher Benoit, lui dire qu'il a entendu Eddie menacer de tout dévoiler, lui dire tout le mal qu'il pense d'Eddie (cet employé qui cherche à partir des MiB) et lui proposer de l'aider à faire disparaitre l'argent, ce qui prouverait sa culpabilité. Mais trop tard, Benoit aura disparu avant que nous n'ayons le temps de faire quoi que ce soit.


![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)   
Les papiers recyclables, dans la poubelle jaune !

Fin de la seconde phase, objectifs atteints !
Nous apprenons plus tard que nous sommes sélectionnés pour la dernière étape, celle de l'intrusion physique. Nous laissons le soin aux premiers de nous faire un write-up, étant arrivés quatrièmes et derniers ;)
Cependant, cette phase était précédée d'encore un peu de Social Engineering, qui s'est passé comme ceci:

## Phase III: récupération et intrusion

La mission est simple: récupérer le raspberry que May, agent infiltré chez SupremIoT, s'apprête à donner à un de ses propres agents. Nous devons récupérer l'objet. L'équipe prépare alors son plan d'action: le nom de code de May est Venom Black Lotus? Guillaume sera alors Ange de Serra, collègue de May, infiltré chez MiB pour récupérer le matériel. Une carte Magic, quelques kanjis dessinés de main de maître par Bill, et Guillaume a une superbe carte de visite.
Il suit May et la rejoint alors qu'elle s'arrête, visiblement dans l'attente d'une personne. 'Oui ?' dit-elle. Guillaume lui dit alors: 'Avoue que tu n'es pas étonnée de me voir. Regarde cette carte discrètement (il lui montre sa carte). Vite, je ne vais pas échapper à la surveillance des MiB bien longtemps.'
Black Lotus lui donne l'objet sans protester. Guillaume repart tranquillement, comme si de rien n'était.

C'est alors que le gars de Digital Security intercepte Guillaume et le force à le suivre. Chemin faisant, Bill vient à la rencontre de Guillaume. Les deux hommes se croisent comme s'il ne se connaissaient pas, personne ne ralentit la cadence. Mais le raspberry est désormais dans les mains de Bill.

Guillaume se retrouve dans la chambre forte de SupremIoT. Scandalisé qu'on le menotte alors qu'il n'a rien volé, c'est une erreur tout ça, il n'a plus qu'à attendre.

Le reste de l'équipe prend alors le gars en filature. Volkmar vient à sa rencontre directement, lui parlant de toutes sortes de choses passionnantes qu'il veut lui vendre, pendant que Eddie fait discrètement une copie de son badge (enfin ça aurait dû se passer comme ça si le matériel avait fonctionné ! :))

Une fois la copie obtenue, l'équipe atteint la chambre forte, libère Guillaume, et procède à une intrusion en règle. Mais ça, c'est une autre histoire...
