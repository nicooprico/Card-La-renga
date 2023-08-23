   <template>
    <div class="album-card">
      <h1>{{ album.title }}</h1>
      <img :src="album.cover" alt="Album Cover" />
      <div class="cd-list">
        <CdItem v-for="cd in album.cds" :key="cd.id" :cd="cd" />
      </div>
    </div>
  </template>
  
  <script>
  import CdItem from './CdItem.vue';
  
  export default {
    props: {
      album: Object
    },
    components: {
      CdItem
    }
  };
  </script>
  
  <style>
  .album-card {
    border: 2px solid #ccc;
    padding: 20px;
    width: 500px;
    text-align: center;
    margin: 20px auto;
    box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.3);
  }
  
  .album-card h1 {
    margin-top: 0;
    font-size: 45px;
    
  }
  
  .album-card img {
    max-width: 100%;
    height: auto;
    margin: 10px 0;
  }
  
  .cd-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }

  
  </style>
  