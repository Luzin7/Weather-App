<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" class="search-bar" placeholder="Tell me where..."/>
      </div>

      <div class="weather-infos">
        <div class="location-box">
          <div class="location">Recife, PE</div>
          <div class="date">Wednesday 05 July 2014</div>
        </div>

        <div class="weather-box">
          <div class="temperature">27°c</div>
          <div class="weather">Hell</div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>

export default {
  name: 'app',
  data(){
    return{
      api_key: '973db35b274b2d5eaa4ba88d11c72dee'
    }
  }
}

</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{}

#app{
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  background-color: #c9e9ff;
  background-size: cover;
  background-position: bottom;

  transition: 0.4s;
}

main{
  min-height: 100vh;
  padding:20px;

  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.25));
}

.search-box{
  text-align: center;
  margin: 0px 0px 20px 0px;
}

.search-box .search-bar{
  display: box;
  width: 70%;
  padding: 10px;

  color: #313131;
  font-size: 20px;

  appearance: none;
  border: none;
  outline: none;
  background: none;
  background-color: rgba(255, 255, 255, .25);
  box-shadow: 2px 4px 0px rgba(0, 0, 0, .25);
  
  border-radius: 60px;
}

.search-box .search-bar:focus{
  color: #227ba2;
  background-color: rgba(255, 255, 255, .4);
  box-shadow: 4px 8px 0px rgba(0, 0, 0, .25);

  transition: 0.4s ease-out;
}

.location-box .location{
  color: #fff;
  font-size: 35px;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 2px rgba(0, 0, 0, 0.25);
}

.location-box .date{
  color: #fff;
  font-size: 25px;
  font-weight: 300;
  text-align: center;
  text-shadow: 1px 2px rgba(0, 0, 0, .25);
}

.weather-box{
  text-align: center;
}

.weather-box .temperature{
  display: inline-block;
  padding: 10px 25px;
  color: #fff;
  font-size: 100px;
  font-weight: 900;

  text-shadow: 1px 2px rgba(0, 0, 0, .25);
  background-color: rgba(255, 255, 255, .25);
  border-radius: 20px;
  margin: 30px 0px;

  box-shadow: 4px 8px 0px rgba(0, 0, 0, .25);
}

.weather-box .weather{
  color: #fff;
  font-size:50px;
  font-weight: 300;
  font-style: italic;

  text-shadow: 1px 2px rgba(0, 0, 0, .25);

}
</style>
