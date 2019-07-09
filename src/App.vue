<template>
  <div id="app">
    <img alt="Vue logo" class="logo" src="./assets/logo.png">
    <HelloWorld :imgList="imgList"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  data() {
    return {
      imgList: [
        'https://cdn.pixabay.com/photo/2017/02/20/18/03/cat-2083492__340.jpg',
        'https://cdn.pixabay.com/photo/2017/01/14/12/59/iceland-1979445__340.jpg',
        'https://cdn.pixabay.com/photo/2016/11/14/04/45/elephant-1822636__340.jpg',
        'https://cdn.pixabay.com/photo/2017/07/18/18/24/dove-2516641__340.jpg',
        'https://cdn.pixabay.com/photo/2016/03/27/22/22/fox-1284512__340.jpg',
        'https://cdn.pixabay.com/photo/2017/05/31/18/38/sea-2361247__340.jpg',
        'https://cdn.pixabay.com/photo/2016/01/08/11/57/butterfly-1127666__340.jpg',
        'https://cdn.pixabay.com/photo/2016/04/20/19/47/wolf-1341881__340.jpg',
        'https://cdn.pixabay.com/photo/2016/12/05/11/39/fox-1883658__340.jpg',
        'https://cdn.pixabay.com/photo/2017/07/24/19/57/tiger-2535888__340.jpg',
        'https://cdn.pixabay.com/photo/2018/07/31/22/08/lion-3576045__340.jpg',
        'https://cdn.pixabay.com/photo/2012/06/19/10/32/owl-50267__340.jpg',
        'https://cdn.pixabay.com/photo/2018/08/12/16/59/ara-3601194__340.jpg',
        'https://cdn.pixabay.com/photo/2017/10/25/16/54/african-lion-2888519__340.jpg',
        'https://cdn.pixabay.com/photo/2018/01/22/14/13/animal-3099035__340.jpg',
        'https://cdn.pixabay.com/photo/2017/02/07/16/47/kingfisher-2046453__340.jpg',
        'https://cdn.pixabay.com/photo/2017/02/28/23/00/swan-2107052__340.jpg',
        'https://cdn.pixabay.com/photo/2016/01/02/16/53/lion-1118467__340.jpg',
        'https://cdn.pixabay.com/photo/2015/11/16/16/28/bird-1045954__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/01/14/30/squirrel-4310069__340.jpg',
        'https://cdn.pixabay.com/photo/2016/12/04/21/58/rabbit-1882699__340.jpg',
        'https://cdn.pixabay.com/photo/2017/10/18/16/08/wolf-2864647__340.jpg',
        'https://cdn.pixabay.com/photo/2017/10/31/07/49/horses-2904536__340.jpg',
        'https://cdn.pixabay.com/photo/2012/10/25/23/52/wolf-62898__340.jpg',
        'https://cdn.pixabay.com/photo/2018/10/08/14/46/bird-3732867__340.jpg',
        'https://cdn.pixabay.com/photo/2017/10/20/10/58/elephant-2870777__340.jpg',
        'https://cdn.pixabay.com/photo/2016/11/12/11/51/forest-1818690__340.jpg',
        'https://cdn.pixabay.com/photo/2017/10/27/20/25/leopard-2895448__340.jpg',
        'https://cdn.pixabay.com/photo/2014/11/28/01/01/jay-548381__340.jpg',
        'https://cdn.pixabay.com/photo/2015/04/10/01/41/fox-715588__340.jpg',
        'https://cdn.pixabay.com/photo/2016/12/13/00/13/rabbit-1903016__340.jpg',
        'https://cdn.pixabay.com/photo/2016/07/10/21/47/cat-1508613__340.jpg',
        'https://cdn.pixabay.com/photo/2014/12/22/10/04/lion-577104__340.jpg',
        'https://cdn.pixabay.com/photo/2018/03/26/20/49/tiger-3264048__340.jpg',
        'https://cdn.pixabay.com/photo/2017/07/22/22/56/tiger-2530158__340.jpg',
        'https://cdn.pixabay.com/photo/2016/04/06/01/32/fuchs-1310826__340.jpg',
        'https://cdn.pixabay.com/photo/2018/01/25/14/12/nature-3106213__340.jpg',
        'https://cdn.pixabay.com/photo/2015/10/12/15/46/fallow-deer-984573__340.jpg',
        'https://cdn.pixabay.com/photo/2018/03/11/20/42/mammals-3218028__340.jpg',
        'https://cdn.pixabay.com/photo/2016/10/21/14/46/norway-1758183__340.jpg',
        'https://cdn.pixabay.com/photo/2019/06/12/15/07/cat-4269479__340.jpg',
        'https://cdn.pixabay.com/photo/2015/11/16/14/43/cat-1045782__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/02/10/25/giraffe-4312090__340.jpg',
        'https://cdn.pixabay.com/photo/2014/04/13/20/49/cat-323262__340.jpg',
        'https://cdn.pixabay.com/photo/2017/11/06/09/53/animal-2923186__340.jpg',
        'https://cdn.pixabay.com/photo/2016/05/02/13/17/wildlife-1367217__340.jpg',
        'https://cdn.pixabay.com/photo/2014/08/29/03/02/horse-430441__340.jpg',
        'https://cdn.pixabay.com/photo/2017/12/11/15/34/lion-3012515__340.jpg',
        'https://cdn.pixabay.com/photo/2014/12/08/17/52/mare-561221__340.jpg',
        'https://cdn.pixabay.com/photo/2019/06/24/20/02/frog-4296784__340.jpg',
        'https://cdn.pixabay.com/photo/2015/03/26/09/54/pug-690566__340.jpg',
        'https://cdn.pixabay.com/photo/2016/12/31/21/22/discus-fish-1943755__340.jpg',
        'https://cdn.pixabay.com/photo/2011/09/27/18/52/sparrow-9950__340.jpg',
        'https://cdn.pixabay.com/photo/2017/06/07/10/47/elephant-2380009__340.jpg',
        'https://cdn.pixabay.com/photo/2017/12/17/15/58/mammal-3024471__340.jpg',
        'https://cdn.pixabay.com/photo/2014/09/16/01/19/girl-447701__340.jpg',
        'https://cdn.pixabay.com/photo/2015/04/20/13/18/animals-731213__340.jpg',
        'https://cdn.pixabay.com/photo/2016/10/10/14/13/dog-1728494__340.png',
        'https://cdn.pixabay.com/photo/2016/05/25/13/55/horses-1414889__340.jpg',
        'https://cdn.pixabay.com/photo/2015/06/08/15/02/pug-801826__340.jpg',
        'https://cdn.pixabay.com/photo/2017/04/14/16/46/red-fox-2230731__340.jpg',
        'https://cdn.pixabay.com/photo/2013/10/17/20/59/horse-197199__340.jpg',
        'https://cdn.pixabay.com/photo/2017/12/10/15/16/white-horse-3010129__340.jpg',
        'https://cdn.pixabay.com/photo/2017/04/11/21/34/giraffe-2222908__340.jpg',
        'https://cdn.pixabay.com/photo/2013/05/30/18/21/tabby-114782__340.jpg',
        'https://cdn.pixabay.com/photo/2016/11/29/10/07/animal-1868911__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/10/21/meadow-4320155__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/07/14/03/fiat-4322521__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/10/52/squirrel-4318302__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/07/37/candles-4317897__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/06/51/library-4317851__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/12/51/palace-4320416__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/02/44/nature-4319662__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/16/42/cornfield-4316900__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/10/28/cabbage-white-4320159__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/06/40/sushi-4317834__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/02/20/22/landscape-4313085__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/16/18/cosmea-4314954__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/06/50/peony-4317848__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/15/45/honey-bee-4314838__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/06/03/lily-4317763__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/01/22/turtles-4317619__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/09/45/train-4320077__340.jpg',
        'https://cdn.pixabay.com/photo/2014/04/14/20/11/japanese-cherry-trees-324175__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/10/02/cormorant-4320134__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/17/13/tulip-4316943__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/21/30/background-4319411__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/21/16/hedgehog-child-4319395__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/06/49/peony-4317847__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/16/16/sparrow-4314952__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/01/14/30/squirrel-4310069__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/06/11/cat-4319756__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/09/58/candytuft-4320103__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/20/59/abendstimmung-4315445__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/15/07/summer-4318824__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/11/50/cat-4320330__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/13/47/horse-4316644__340.jpg',
        'https://cdn.pixabay.com/photo/2019/06/25/13/06/fiat-4298163__340.jpg',
        'https://cdn.pixabay.com/photo/2019/06/25/21/07/squirrel-4299060__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/20/54/jackdaw-4321240__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/07/15/08/margarite-4322656__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/02/10/25/giraffe-4312090__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/08/01/04/caterpillar-4323586__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/10/04/stork-4318178__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/18/07/coil-4320892__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/07/02/05/moon-4321596__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/10/31/pink-4316319__340.jpg',
        'https://cdn.pixabay.com/photo/2019/06/29/06/30/weigelien-4305542__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/12/28/hay-4318472__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/10/01/rose-4320119__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/21/04/evening-4319383__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/08/01/21/water-4323621__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/12/38/chihuahua-4320391__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/09/57/great-crested-grebe-4320098__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/10/01/horse-4320124__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/13/11/heart-flower-4318550__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/17/28/facade-4320830__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/07/01/34/the-earth-4321567__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/14/23/landscape-4316684__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/02/20/16/lake-4313078__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/02/17/52/turtles-4312790__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/13/26/cherries-4320487__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/23/18/atlas-moth-4321450__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/15/07/summer-4318826__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/09/41/national-history-museum-4314035__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/12/45/background-4320397__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/07/21/50/bouquet-4323374__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/16/20/superb-thread-4314962__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/18/07/cherries-4317035__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/16/48/cherry-4316913__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/15/44/tree-mallow-4314836__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/11/44/squirrel-4316409__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/03/15/42/crow-4314822__340.jpg',
        'https://cdn.pixabay.com/photo/2019/06/29/18/51/rails-4306770__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/10/20/roses-4316307__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/14/24/landscape-4316685__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/02/01/51/cosmea-4311192__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/07/06/33/man-4321831__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/17/11/giraffe-4316937__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/04/17/06/flowers-4316924__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/05/13/08/cows-4318543__340.jpg',
        'https://cdn.pixabay.com/photo/2019/07/06/13/31/heart-4320491__340.jpg',
        'https://cdn.pixabay.com/photo/2019/06/29/16/28/mouse-4306520__340.jpg',
      ],
      
    }
  },
  components: {
    HelloWorld
  },
  mounted() {
  },
  methods: {
  }
}
</script>


<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.logo {
  animation: scale 2s backwards infinite;
}
@keyframes scale {
  form {
    transform: scale(100%);
  }
  50% {
    transform: scale(0);
  }
  to {
    transform: scale(100%);
  }
}
</style>
