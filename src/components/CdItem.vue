    <template>
    <div class="cd-item">
      <img :src="cd.cover" alt="CD Cover" />
      <h2>{{ cd.title }}</h2>
      <p>{{ cd.description }}</p>
      <div class="rating">
        <span v-for="star in 5" :key="star" class="star" :class="{ filled: star <= cd.rating }">&#9733;</span>
      </div>
      <div class="button"> Comprar </div>
      
    </div>
  </template>
  
  <script>
  export default {
    props: {
      cd: Object
    }
  };
  </script>
  
  
  <style>
.cd-item {
  border: 1px solid #ccc;
  padding: 10px;
  width: calc(50% - 10px);
  margin-bottom: 20px;
  text-align: center;
  box-shadow: 0px 0px 3px rgba(0, 0, 0, 0.2);
}


.cd-item img {
  max-width: 100%;
  height: auto;
  margin-bottom: 10px;
}

.cd-item p {
  font-size: 14px;
  
  
}

.cd-item h2 {
  font-size: 18px;
  font-weight: bold;
}


.rating {
  margin-top: 10px;
}

.star {
  font-size: 20px;
  color: #ccc;
  cursor: pointer;
  transition: color 0.3s;
}

.star.filled {
  color: gold;
}

.button {
  background-color: #3498db;
  color: #fff;
  border: none;
  padding: 5px 5px;
  border-radius: 4px;
  cursor: pointer;
  transition: background-color 0.3s, color 0.3s;
}

.button:hover {
  background-color: #2980b9;




}
</style>

  