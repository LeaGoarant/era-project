<template>
  <v-app>
    <v-main class="app">
      <v-row justify="start" no-gutters>
        <v-col cols="auto" class="mr-0 pr-0">
          <v-img alt="logoEra" src="./assets/logo-era.jpg" height="150" width="150"></v-img>
        </v-col>
        <v-col cols="auto" class="ml-0 pl-0">
          <v-img alt="kittens" src="./assets/chat-era.webp" height="150" width="400"></v-img>
        </v-col>
        <v-col cols="3" class="ml-0 pl-0 mr-0 pr-0">
          <v-img alt="kittens2" src="./assets/chat-era2.webp" height="150" width="150"></v-img>
        </v-col>
        <v-col cols="4" class="align-self-center ml-0 pl-0 mr-4" style="color: #9c726a; font-style: italic">
          « C’est impossible, dit la Fierté, C’est risqué, dit l’Expérience, 
          C’est sans issue, dit la Raison, Essayons, murmure le Cœur » William Arthur Ward 
        </v-col>
      </v-row>
      <v-app-bar color="#a796be" height="40px" flat>
        <v-container>
          <v-row justify="space-between">
            <v-col>
              <v-btn plain @click="App">Accueil</v-btn>
            </v-col>
            <v-col>
              <v-btn plain @click="Adoptions">Adoptions</v-btn>
            </v-col>
            <v-col>
              <v-btn plain>Bénévolat</v-btn>
            </v-col>
            <v-col>
              <v-btn plain>S'informer</v-btn>
            </v-col>
            <v-col>
              <v-btn plain>Faire un don</v-btn>
            </v-col>
            <v-col>
              <v-btn plain>Contact</v-btn>
            </v-col>
          </v-row>
        </v-container>
      </v-app-bar>
      <v-spacer></v-spacer>
      <v-container>
        <v-card style="background-color: #dbd3d3" class="mt-5">
          <v-card-title style="color: #01b1af">La philosophie ERA</v-card-title>
          <v-card-text style="color: black">
            Association fondée le 23 décembre 2014 dans le but d’offrir assistance et soins aux chats abandonnés de 
            l’agglomération Strasbourgeoise et de leur assurer un avenir meilleur. L’association milite également en 
            faveur de la stérilisation des chats errants, seule solution d’avenir pour nos compagnons les félins comme 
            pour nous, humains. ERA c’est depuis sa création, plus 5500 chats pris en charge, une trentaine de 
            bénévoles passionnés et dévoués à la cause. L’association fonctionne essentiellement grâce à la générosité 
            et à l’implication de son réseau de familles d’accueil.
            <br/>
            <br/>
            Notre association est née du désir d'apporter une gestion éthique de la population féline.
            Chez ERA nous pensons que chaque chat a sa chance de trouver sa famille. Qu'il soit "beau" ou non, 
            qu'il soit malade ou non, qu'il soit handicapé ou parfaitement valide, tous ont leur place au sein 
            de l'association. Nous refusons toute euthanasie de confort et réservons cet acte exclusivement pour 
            les cas vétérinaires graves et sans espoir. Si nous venons à manquer de places en accueil, nous 
            stoppons les prises en charge mais ne déciderons jamais de la fin de vie d'un animal sain.
          </v-card-text>
        </v-card>
        <v-card style="background-color: #dbd3d3" class="mt-5">
          <v-card-title style="color: #01b1af">ERA en chiffres</v-card-title>
          <v-card-text style="color: black">
            <p><b>Les principaux chiffres ERA en 2019</b></p> 
            <v-list>
              <v-list-item-content>
                <v-list-item-title>
                  Côté chats :
                </v-list-item-title>
                <v-list-item-subtitle>
                  Nombre de chats pris en charge : 1203
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  Nombre de chats adoptés : 1030
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  Nombre de chats ayant retrouvé leur propriétaire : 6
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  Nombre de chats relâchés sur site après identification et stérilisation : 112
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                 Nombre de décès et euthanasies : 107
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list>
            <v-list>
              <v-list-item-content>
                <v-list-item-title>
                  Côté finances : 
                </v-list-item-title>
                <v-list-item-title>
                  Recettes : 
                </v-list-item-title>
                <v-list-item-subtitle>
                  - Dons et cotisations 2018 : 59 270 €
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  - Adoptions : 111 705 €
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  - Ventes : 27 534 € 
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  - Autres produits d'exploitation : 15 261 € (dont appel de fond pour la construction du refuge)
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                 - Montant des abandons de frais des bénévoles : 8 601 €
                </v-list-item-subtitle>
                <v-list-item-title>
                 Dépenses : 
                </v-list-item-title>
                <v-list-item-subtitle>
                  Montant des frais engagés par l’association : 229 849 € dont :
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  - Frais vétérinaires : 163 010 €
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  - Frais d'alimentation pour les animaux : 12 288 € 
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                  - Achats destinées à la revente : 16 664 €
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                 - Petit matériel et fournitures d'entretien : 7 529 €
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                 - Location immobilière : 2 491 €
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list>
            <p>Nous tenons à adresser nos plus sincères et chaleureux remerciements à tous nos bénévoles, ceux qui
            sont là depuis toujours et ceux qui nous rejoignent pour leur immense travail et leurs efforts 
            quotidiens pour prendre soins de ces êtres délaissés. Chacun à sa manière et en fonction de ses 
            possibilités, c’est l’unité de toutes ces bonnes volontés qui nous permet d’aller toujours plus loin 
            et de s’adapter encore et toujours. Merci aux vétérinaires qui nous soutiennent dans notre action en 
            nous accordant des tarifs avantageux et en prodiguant des soins attentionnés à nos loulous, leur aide 
            est précieuse. Merci à la fourrière animale de Strasbourg, la SACPA avec qui nous collaborons tout au 
            long de l'année pour récupérer, en partage avec la SPA les animaux que personne ne vient réclamer.
            Merci à tous nos adhérents et donateurs, sans vous bien sûr rien ne serait possible et chaque 
            soutien donne une chance à un animal supplémentaire de connaître une nouvelle vie heureuse. Enfin, 
            merci à tous ceux qui en 2018 ont choisi de donner une chance à animal qui n’en avait pas eu 
            jusque-là en lui ouvrant les portes de son foyer.</p>
            <p style="font-size: 11px">
              ERA est une association reconnue d’intérêt général, ainsi chaque don ou adhésion ouvre droit à 
              une déduction fiscale à hauteur de 66% de vos dons et dans la limite de 20% de votre revenu imposable. 
              Pour les entreprises, les dons ouvrent droit à une déduction fiscale à hauteur de 60 % dans la limite 
              de 5/00 (5 pour 1000) du chiffre d’affaire annuel HT. (voir au dos de la brochure)
            </p>
          </v-card-text>
        </v-card>
      </v-container>
    </v-main>
    <v-footer style="background-color: #a8a4a1" height="120px">
      <v-container>
        <v-row>
          <v-col cols="5" style="color: white">
            ©2014 - ERA Association Strasbourg - TOUS DROITS RESERVES 
            <br/> 
            Mentions légales
          </v-col>
          <v-col cols="6" style="color: white">
            Association inscrite au registre des associations du tribunal d'instance de Strasbourg,
            Volume 92, Folio 324. n° SIRET : 808 946 883 00010
          </v-col>
          <v-col cols="1" class="align-self-end justify-content-end">
            <v-icon>mdi-facebook</v-icon>
            <br/>
            <v-icon>mdi-youtube</v-icon>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
import Adoptions from './components/Adoptions'
export default {
  name: 'App',
  components: {
    Adoptions
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
  .app {
    background-color: #e9e5db;
  }
</style>
