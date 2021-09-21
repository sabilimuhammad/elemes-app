<template>
  <div class="container mx-auto items-center">
    <header class="items-center justify-between pt-20 flex">
      <div class="w-5/12">
        <h1 class="text-primary">Good Food Us Good Mood</h1>
        <p class="py-8">
          I would think that conserving our natural resources should be a
          conservative position: Not to waste food, and not to throw away a lot
          of the food that we buy.
        </p>
        <div>
          <button class="btn bg-primary rounded-3xl mr-4 shadow-lg">
            Daftar Sekarang
          </button>
          <button class="btn-light bg-light-gray rounded-3xl">About Us</button>
        </div>
      </div>
      <div>
        <div>
          <div
            class="w-96 h-96 bg-opacity-75 rounded-full bg-light-gray relative"
          >
            <div class="absolute pt-8 pl-8">
              <img class="h-80 w-80" src="../assets/images/image.png" />
            </div>
          </div>
          <div class="relative px-4 -mt-16">
            <div class="wrapper-transparent p-6 rounded-xl shadow-lg flex">
              <div class="mr-2">
                <img class="h-12 w-12" src="../assets/images/image.png" />
              </div>
              <div>
                <h6>Green Salad Tomato</h6>
                <p>Tomato</p>
                <div>
                  <img src="../assets/images/icons/stars-5.svg" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
    <div class="relative py-16">
      <h4>
        Browser Our Category
        <h4 class="text-primary">Receipt</h4>
      </h4>
      <div class="pt-8">
        <div class="flex gap-x-4">
          <div
            v-for="(cat, i) in cats"
            :key="`cats-${i}`"
            class="h-48 w-52 rounded-3xl"
            :class="cat.color"
          >
            <div class="p-4">
              <img class="rounded-lg" :src="cat.icon" />
              <h6>{{ cat.name }}</h6>
              <span>{{ cat.amount }}</span>
            </div>
          </div>
        </div>
      </div>
      <div class="absolute py-8 right-0">
        <button class="btn mr-4 bg-primary rounded-3xl">prev</button>
        <button class="btn bg-primary rounded-3xl">next</button>
      </div>
    </div>
    <div class="py-16">
      <h4>
        Browser Our Trending
        <h4 class="text-primary">Receipt</h4>
      </h4>
      <div class="grid grid-cols-1 md:grid-cols-4 lg:grid-cols-4 pt-8 gap-4">
        <div
          v-for="(card, i) in cards"
          :key="`cards-${i}`"
          class="h-58 w-48 p-2 rounded-3xl shadow-lg md:w-auto lg:w-auto"
          :class="card.color"
        >
          <div class="p-4">
            <img class="h-24 w-24 rounded-lg" :src="card.picture"/>
            <h6>{{ card.title }}</h6>
            <p class="text-primary">{{ card.type }}</p>
            <img :src="card.ratings" />
          </div>
        </div>
      </div>
      <div class="relative text-center pt-8 pb-28">
        <button class="btn bg-primary text-center rounded-3xl mr-4">
          ALL Receipt
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      innerStyles: {},
      step: '',
      cats: [
        {
          icon: require('@/assets/images/icons/Frame.svg'),
          name: 'Cupcake',
          amount: '22 items',
          color: 'bg-secondary-shadow',
        },
        {
          icon: require('@/assets/images/icons/pizza.svg'),
          name: 'Pizza',
          amount: '22 items',
          color: 'bg-secondary-shadow',
        },
        {
          icon: require('../assets/images/icons/kebab.svg'),
          name: 'Kebab',
          amount: '22 items',
          color: 'bg-secondary-darkest-shadow',
        },
        {
          icon: require('../assets/images/icons/salmon.svg'),
          name: 'Salmon',
          amount: '22 items',
          color: 'bg-primary-lighten-shadow',
        },
        {
          icon: require('../assets/images/icons/doughnut.svg'),
          name: 'Doughnut',
          amount: '22 items',
          color: 'bg-secondary-darkest-shadow',
        },
      ],
      cards: [
        {
          picture: require('../assets/images/pexels-brett-pizza.png'),
          title: 'Paperoni',
          type: 'Pizza',
          ratings: require('../assets/images/icons/stars-5.svg'),
          color: 'bg-secondary-shadow',
        },
        {
          picture: require('../assets/images/pexels-daria-shev.png'),
          title: 'Pizza Meat',
          type: 'Pizza',
          ratings: require('../assets/images/icons/stars-5.svg'),
          color: 'bg-secondary-shadow',
        },
        {
          picture: require('../assets/images/pexels-nishant-kebab.png'),
          title: 'Kebab',
          type: 'Kebab',
          ratings: require('../assets/images/icons/stars-3.svg'),
          color: 'bg-secondary-darkest-shadow',
        },
        {
          picture: require('../assets/images/pexels-olga-lion.png'),
          title: 'Salmon Roll',
          type: 'Salmon',
          ratings: require('../assets/images/icons/stars-5.svg'),
          color: 'bg-secondary-purple-shadow',
        },
        {
          picture: require('../assets/images/pexels-oleg-mag.png'),
          title: 'Cupcake Choco',
          type: 'Cupcae',
          ratings: require('../assets/images/icons/stars-5.svg'),
          color: 'bg-primary-shadow',
        },
        {
          picture: require('../assets/images/pexels-alena-donut.png'),
          title: 'Doughnut Milk',
          type: 'Doughnut',
          ratings: require('../assets/images/icons/stars-5.svg'),
          color: 'bg-primary-lighten-shadow',
        },
        {
          picture: require('../assets/images/pexels-karley.png'),
          title: 'Doughnut Unicorn',
          type: 'Doughnut',
          ratings: require('../assets/images/icons/stars-5.svg'),
          color: 'bg-primary-lighten-shadow',
        },
        {
          picture: require('../assets/images/pexels-polina-tank.png'),
          title: 'Kathi Kebab',
          type: 'Kebab',
          ratings: require('../assets/images/icons/stars-5.svg'),
          color: 'bg-secondary-darkest-shadow',
        },
      ],
    }
  },
}
</script>