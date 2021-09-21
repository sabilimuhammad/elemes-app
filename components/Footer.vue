<template>
  <div class="container mx-auto bg-secondary-shadow justify-between rounded-3xl">
      <div class="grid grid-cols-1 lg:grid-cols-2 xl:grid-cols-4">
          <div class="m-8">
            <img src="@/assets/images/icons/logo.svg" />
            <p class="text-gray-400 text-xs py-4">
              Jl. Prof. DR. Satrio No.7, RT.3/RW.3, Karet Kuningan, Kecamatan
              Setiabudi, Kota Jakarta Selatan, Daerah Khusus Ibukota Jakarta
              12950
            </p>
            <div class="flex">
              <img src="@/assets/images/icons/email-rounded.svg" />
              <img class="mx-4" src="@/assets/images/icons/phone-rounded.svg" />
              <img src="@/assets/images/icons/ig.svg" />
            </div>
          </div>
          <div class="m-8">
            <h6>Categories</h6>
            <ul class="list-none">
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                Cupcake
              </li>
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                Pizza
              </li>
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                Kebab
              </li>
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                Salmon
              </li>
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                Doughnut
              </li>
            </ul>
          </div>
          <div class="m-8">
            <h6 class="footer-item-title">About Us</h6>
            <ul class="list-none">
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                About Us
              </li>
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                FAQ
              </li>
              <li class="footer-links-item text-gray-400 hover:text-gray-600">
                Report Problem
              </li>
            </ul>
          </div>
        <div class="m-8">
          <h6>Newsletter</h6>
          <p class="text-gray-400 text-xs py-2">
            Get now free 50% discount for all products on your first order
          </p>
          <div class="mt-1 w-20 flex rounded-md shadow-sm">
            <input
              type="text"
              class="h-8 focus:ring-indigo-500 focus:border-indigo-500 flex-1 block rounded-none rounded-l-md sm:text-sm border-gray-300"
              placeholder=" Your email address"
            />
            <button
              class="inline-flex items-center px-3 rounded-r-md border border-r-0 border-gray-300 bg-primary text-white text-sm"
            >
              SEND
            </button>
          </div>
          <button class="flex items-center py-2" type="text">
            <img
              class="mr-4"
              src="@/assets/images/icons/email.svg"
            />elemesid@gmail.com
          </button>
          <button class="flex items-center" type="text">
            <img
              class="mr-4"
              src="@/assets/images/icons/phone.svg"
            />0888-1111-2222
          </button>
        </div>
      </div>
  </div>
</template>

<script>
export default {};
</script>