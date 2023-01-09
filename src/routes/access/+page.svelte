<div class="access-container">
    <h1 class="center">
      Sample location:
    </h1>
    <div id="googleMap" style="width:70%;height:400px;" class="map"></div>
  
    <div class="center flex">
      <div >
        <img class="logo" src="" alt="" />
      </div>
      <div id="info" class="center info jp">
        <p>〒529−1422</p>
        <p>滋賀県東近江市五個荘小幡町87−１</p>
        <p class="smaller">五個荘駅から徒歩約10分</p>
  
      </div>
    </div>
  </div>

  <script defer>
    function myMap() {
    var mapProp= {
      center:new google.maps.LatLng(35.1229951444847, 136.10275043992064),
      zoom:17,
    };
    var map = new google.maps.Map(document.getElementById("googleMap"),mapProp);
    }
</script>
  