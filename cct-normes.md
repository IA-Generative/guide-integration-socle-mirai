# **Cadre de Cohérence Technique (CCT) du socle d’IA et Guide d’intégration “Socle MIRAI“**

**Version : VERSION EN COURS D’ELABORATION**

**Date :** 17/03/2025

**Auteur :** Direction de la transformation numérique du Ministère de l’Intérieur et des Outre-Mer.


Cette version RFC (request for comment) vous permet de proposer vos commentaires de plusieurs manières:
- faire des issues
- utiliser le fichier de relecture proposé
[Fichier pour commentaires](./gabarit-pour-commentaires.ods)
 et l’envoyer à : [dnum-architecture-entreprise@interieur.gouv.fr](mailto:dnum-architecture-entreprise@interieur.gouv.fr)
## Les normes industrielles, institutionnelles applicables<a id="les-normes-industrielles-institutionnelles-applicables"></a>

La conception de système d’information dans le cadre de l’État est encadrée par un ensemble de recommandations ou règles à mettre en œuvre.  Ces normes sont citées ci-dessous. Le lecteur est invité à vérifier qu’il dispose des versions les plus à jour.

| Normes industrielles                                                                     | Kubernetes : [https://kubernetes.io/fr/](https://kubernetes.io/fr/)<br>ArgoCD : [https://argo-cd.readthedocs.io/en/stable/](https://argo-cd.readthedocs.io/en/stable/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Guides & outils pour la conception                                                     | DSFR : Design System FR. La charte internet de l’État ( qui intègre le RGAA )<br>[https://www.systeme-de-design.gouv.fr/](https://www.systeme-de-design.gouv.fr/)<br>Guide d’éco conception : [https://ecoresponsable.numerique.gouv.fr/publications/referentiel-general-ecoconception/](https://ecoresponsable.numerique.gouv.fr/publications/referentiel-general-ecoconception/)<br><br>Divers guides de conceptions logiciels:<br>https://[guides.etalab.gouv.f](https://guides.etalab.gouv.fr/accueil.html)r<br>[https://](https://catalogue.numerique.gouv.fr)[catalogue.numerique.gouv.fr](https://catalogue.numerique.gouv.fr)<br>[https://](https://schema.gouv.fr)[schema.gouv.fr](https://schema.gouv.fr)<br>[https://](https://code.gouv.fr)[code.gouv.fr](https://code.gouv.fr) |
| Cadres de pratiques de conception et de conduite de projet agile                       | [https://www.numerique.gouv.fr/actualites/guide-pour-allier-agilite-et-securite-numeriques/](https://www.numerique.gouv.fr/actualites/guide-pour-allier-agilite-et-securite-numeriques/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Logiciel libre                                                                         | Socle InterMinistériel des Logiciels Libres ( SILL) de par sa fonction de source pour le référentiel de produits du CCT Ministériel : [https://sill.etalab.gouv.fr/fr/software](https://sill.etalab.gouv.fr/fr/software)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Normes interMinistérielles de conception de solutions                                  | Doctrine cloud de l’état : [https://www.legifrance.gouv.fr/circulaire/id/45205](https://www.legifrance.gouv.fr/circulaire/id/45205)<br>Référentiel Général d’Accessibilité pour les Administrations :<br>[https://accessibilite.numerique.gouv.fr/](https://accessibilite.numerique.gouv.fr/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Référentiel Général de Sécurité, en association avec le règlement européen et l’EIDAS. | [https://www.ssi.gouv.fr/entreprise/reglementation/confiance-numerique/liste-des-documents-constitutifs-du-rgs-v-2-0/](https://www.ssi.gouv.fr/entreprise/reglementation/confiance-numerique/liste-des-documents-constitutifs-du-rgs-v-2-0/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Référentiel Général de Gestion des Archives                                            | [https://www.ssi.gouv.fr/entreprise/reglementation/confiance-numerique/le-reglement-eidas/](https://www.ssi.gouv.fr/entreprise/reglementation/confiance-numerique/le-reglement-eidas/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Référentiel Général de Gestion des Archives                                            | [https://francearchives.fr/fr/circulaire/R2GA_2013_10](https://francearchives.fr/fr/circulaire/R2GA_2013_10)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| règlement européen sur la protection des données personnelles                          | [https://www.cnil.fr/fr/reglement-europeen-protection-donnees](https://www.cnil.fr/fr/reglement-europeen-protection-donnees)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| L’IA ACT (réglement européen)                                                          | [https://digital-strategy.ec.europa.eu/fr/policies/regulatory-framework-ai](https://digital-strategy.ec.europa.eu/fr/policies/regulatory-framework-ai)<br>[https://www.cnil.fr/fr/entree-en-vigueur-du-reglement-europeen-sur-lia-les-premieres-questions-reponses-de-la-cnil](https://www.cnil.fr/fr/entree-en-vigueur-du-reglement-europeen-sur-lia-les-premieres-questions-reponses-de-la-cnil)                                                                                                                                                                                                                                                                                                                                                                                          |



****

## Liens vers autres contenus utiles(informatif)<a id="liens-vers-autres-contenus-utilesinformatif"></a>

****

<https://kubernetes.io/fr/>

<https://www.rancher.com/products/k3s>

https\://www\.redhat.com/en/technologies/cloud-computing/openshift

<https://argo-cd.readthedocs.io/en/stable/>

<https://www.redhat.com/en/topics/microservices/what-is-a-service-mesh>

https\://www\.redhat.com/en/topics/devops/what-is-gitops

<https://www.cloudcomputingpatterns.org/>

<https://12factor.net/fr/>

<https://tanzu.vmware.com/content/blog/beyond-the-twelve-factor-app>

<https://www.techworld-with-nana.com/devops-bootcamp>

<https://ecoresponsable.numerique.gouv.fr/publications/bonnes-pratiques/bonnes-pratiques/#bonnes-pratiques-services-numeriques>

****

La documentation sur le CloudPI :

<https://pi.interieur.rie.gouv.fr/> ( accessible via le rie uniquement )

<https://cloud-pi-native.fr/>

<https://github.com/Cloud-pi-Native/>
