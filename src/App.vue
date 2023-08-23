<template>
  <div class="app">
    <AlbumCard :album="albumData" />
  </div>
</template>

<script>
import AlbumCard from './components/AlbumCard.vue';

export default {
  components: {
    AlbumCard
  },
  data() {
    return {
      albumData: {
        title: 'LA RENGA',
        cover: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/98/La_Renga_logo.svg/640px-La_Renga_logo.svg.png',
        cds: [
          {
            id: 1,
            title: 'Despedazado por mil partes',
            description: 'Despedazado por mil partes es el cuarto álbum de la banda de rock argentina La Renga, editado en octubre de 1996.',
            cover: 'https://m.media-amazon.com/images/I/61ga13jIa3L._UF1000,1000_QL80_.jpg',
            rating: 5
          },
          {
            id: 2,
            title: 'Pesados Vestigios',
            description: 'Pesados Vestigios es el undécimo álbum editado por la banda de Rock La Renga. Lanzado el 17 de diciembre de 2014.',
            cover: 'https://www.cmtv.com.ar/tapas-cd/larengapesadosvestigios.webp',
            rating: 5
          },
          {
            id: 2,
            title: 'Algun Rayo',
            description: 'Algún rayo es el décimo álbum realizado por la banda de hard rock La Renga. Fue presentado el sábado 18 de diciembre de 2010.',
            cover: 'https://www.cmtv.com.ar/tapas-cd/larengaalgunrayo.webp',
            rating: 5
          },
          {
            id: 2,
            title: 'La esquina del infinito',
            description: 'Es el sexto álbum grabado por la banda de Hard Rock La Renga. Es considerado la obra cumbre del grupo. Lanzado el 11 de agosto de 2000',
            cover: 'https://www.cmtv.com.ar/tapas-cd/rengaesquina.webp',
            rating: 4
          },
          {
            id: 2,
            title: 'Insoportablemente vivo',
            description: 'Insoportablemente en vivo, es el séptimo álbum de la banda. Fue grabado en el concierto dado en el estadio C.A. Huracán el 19 de mayo de 2001',
            cover: 'https://upload.wikimedia.org/wikipedia/en/0/0d/Insoportablemente_Vivo.jpg',
            rating: 5
          },
          {
            id: 2,
            title: 'Detonador de sueños',
            description:'Detonador de sueños es el octavo álbum realizado por la Banda de Hard Rock La Renga. Fue presentado el 8 de noviembre de 2003 en el estadio Chateau Carreras',
            cover: 'https://upload.wikimedia.org/wikipedia/en/d/da/Detonador_De_Suenos.jpg',
            rating: 4
          }
        ]
      }
    };
  }
};
</script>



