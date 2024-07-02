<template>
  <div>
    <div class="sticky top-0 bg-slate-200 pb-5" style="z-index: 999">
      <div class="flex justify-between md:px-11 px-5 pt-2">
        <div class="flex gap-5 text-md justify-end items-end">
          <a href="#" class="font-black text-xl">
            Foody<span class="text-yellow-500">.</span>
          </a>
          <!-- navbar -->
          <div class="hidden md:block space-x-5">
            <a href="#" class="pl-2 font-medium text-slate-400 focus:text-black"
              >Home</a
            >
            <a href="#aa" class="text-slate-400 focus:text-black"
              >How It Works</a
            >
            <a href="#feature" class="text-slate-400 focus:text-black"
              >Features</a
            >
            <a href="#price" class="text-slate-400 focus:text-black">Pricing</a>
            <a href="#" class="text-slate-400 focus:text-black">FAQs</a>
          </div>
        </div>
        <div class="pt-2 flex items-center space-x-2">
          <button
            type="button"
            class="bg-yellow-500 text-white font-semibold lg:px-5 lg:py-3 px-3"
          >
            sign up
          </button>
          <button
            class="bg-slate-400 p-2 rounded-lg md:hidden block"
            @click="navshow = !navshow"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-list text-white"
              viewBox="0 0 16 16"
            >
              <path
                fill-rule="evenodd"
                d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5z"
              />
            </svg>
          </button>
        </div>
      </div>
      <Transition name="slide-fade">
        <div
          v-if="navshow"
          class="pl-5 space-y-3 pt-5 md:hidden block absolute bg-slate-200 w-full pb-5"
        >
          <a href="#" class="block">Home</a>
          <a href="#aa" class="block">How It Works</a>
          <a href="#feature" class="block">Features</a>
          <a href="#price" class="block">Pricing</a>
          <a href="#" class="block">FAQs</a>
        </div></Transition
      >
    </div>
    <div class="h-screen bg-slate-200">
      <div class="">
        <div
          class="md:grid md:grid-cols-2 gap-10 xl:px-20 md:px-10 xl:pt-0 md:pt-32 md:gap-0"
        >
          <div
            class="flex items-center justify-center xl:pl-32 md:pl-0 md:px-0 px-5"
          >
            <div>
              <div
                class="xl:text-6xl lg:text-4xl font-bold xl:pb-20 pb-2 md:text-2xl md:pt-0 pt-12 text-xl md:text-left"
              >
                Our food site Makes it easy to find local food
              </div>
              <div class="lg:text-2xl md:text-lg text-xs">
                Imagine you don,t need a diet because we provide healthy and
                delicious food for you! We are providing the best food delivery
                services.
              </div>
              <div class="pt-10 text-center md:text-start">
                <button
                  type="button"
                  class="xl:mr-10 bg-yellow-500 xl:px-14 xl:text-xl font-semibold text-white xl:py-5 xl:rounded-3xl md:mr-5 md:px-5 md:text-lg md:py-3 md:rounded-2xl px-2 py-2 rounded-xl mr-4"
                >
                  Get Started
                </button>
                <button
                  type="button"
                  class="xl:px-14 xl:py-4 border-black xl:text-xl font-semibold border-4 xl:rounded-3xl md:px-5 md:text-lg md:py-2 md:rounded-2xl px-2 py-1 rounded-xl mr-4"
                >
                  Order Now
                </button>
              </div>
            </div>
          </div>

          <div
            class="flex xl:justify-center md:justify-end justify-center items-center"
          >
            <div class="relative hidden md:block">
              <div class="absolute inset-6 -translate-x-24 -translate-y-20">
                <div
                  class="xl:h-32 xl:w-72 md:w-40 md:h-20 bg-white bg-opacity-80 backdrop-blur-xl rounded-2xl"
                >
                  <div class="flex items-center xl:pt-6 md:pt-4 pl-4 gap-3">
                    <img
                      src="./assets/img/dietary-salad-with-chicken-avocado-cucumber-tomato-chinese-cabbage.jpg"
                      alt=""
                      class="xl:w-20 xl:h-20 md:h-12 md:w-12 rounded-full object-cover"
                    />
                    <h1 class="md:text-xs xl:text-base">
                      Lorem ipsum dolor sit amet consectetur.
                    </h1>
                  </div>
                </div>
              </div>

              <div
                class="absolute inset-6 2xl:translate-x-96 xl:translate-x-64 xl:-translate-y-64 lg:translate-x-28 lg:-translate-y-52 md:translate-x-24 md:-translate-y-44 shadow-2xl"
              >
                <div
                  class="xl:h-32 xl:w-72 md:w-40 md:h-20 bg-white bg-opacity-80 backdrop-blur-xl rounded-2xl"
                >
                  <div class="flex items-center xl:pt-6 md:pt-4 pl-4 gap-3">
                    <img
                      src="./assets/img/dietary-salad-with-chicken-avocado-cucumber-tomato-chinese-cabbage.jpg"
                      alt=""
                      class="xl:w-20 xl:h-20 md:h-12 md:w-12 rounded-full object-cover"
                    />
                    <h1 class="md:text-xs xl:text-base">
                      Lorem ipsum dolor sit amet consectetur.
                    </h1>
                  </div>
                </div>
              </div>

              <div
                class="absolute xl:inset-6 xl:translate-x-40 xl:translate-y-24 lg:translate-x-32 md:translate-x-20 md:translate-y-24 shadow-2xl"
              >
                <div
                  class="xl:h-52 xl:w-72 md:w-40 bg-white bg-opacity-80 backdrop-blur-xl rounded-2xl shadow-2xl"
                >
                  <div class="xl:-translate-y-10 md:-translate-y-6">
                    <div class="flex justify-center">
                      <img
                        src="./assets/img/tom-yum-kung-thai-hot-spicy-soup-shrimp-with-lemon-grass-lemon-galangal-chilli-wooden-table-thailand-food.jpg"
                        alt=""
                        class="w-12 h-12 rounded-full object-cover shadow-2xl"
                      />
                    </div>
                    <h1 class="text-center xl:text-2xl font-bold">Burger</h1>
                    <h1 class="text-center xl:pt-2 xl:text-base md:text-xs">
                      ⭐⭐⭐⭐
                    </h1>
                    <h1 class="text-center xl:text-xl md:text-sm font-semibold">
                      Tom/Mirk <br />
                      7 oriebal UM, Pa pi ka
                    </h1>
                  </div>
                </div>
              </div>
            </div>
            <img
              src="./assets/img/crispy-mixed-pizza-with-olives-sausage.jpg"
              alt=""
              class="mt-10 md:h-2/3 h-60 object-cover rounded-3xl bg-cover shadow-2xl"
            />
          </div>
        </div>
      </div>
    </div>
    <!-- Features -->
    <div class="md:h-screen">
      <div>
        <div class="text-center pt-16" id="feature">
          <div class="text-5xl font-bold pb-6">Features</div>
          <div class="text-xl font-medium text-slate-400">
            This lesson provides a basic framework for conducting a recipe
            demonstration
          </div>
        </div>
        <div
          class="md:grid md:grid-cols-3 2xl:gap-56 lg:gap-10 md:gap-0 gap-3 pt-20"
        >
          <div class="flex justify-center 2xl:py-36 md:py-24">
            <div class="md:pb-0 pb-10">
              <img
                src="./assets/img/crispy-mixed-pizza-with-olives-sausage.jpg"
                alt=""
                class="xl:h-56 lg:h-44 h-36 ml-20 rounded-3xl xl:ml-16 lg:ml-14 md:ml-12 object-cover"
              />
              <div class="pt-3">
                <h1 class="text-2xl text-center font-bold">Discount Boucher</h1>
                <h2 class="text-xl text-center">
                  Phasollus risus turpis sit arnot magna non.
                </h2>
              </div>
            </div>
          </div>
          <div
            class="flex justify-center 2xl:py-32 md:py-24 rounded-3xl md:shadow-lg md:pb-0 pb-10"
          >
            <div class="">
              <img
                src="./assets/img/dietary-salad-with-chicken-avocado-cucumber-tomato-chinese-cabbage.jpg"
                alt=""
                class="xl:h-56 lg:h-44 h-36 ml-16 rounded-3xl xl:ml-3 md:ml-8 object-cover"
              />
              <div class="pt-6">
                <h1 class="text-2xl text-center font-bold">
                  Fresh healthy Food
                </h1>
                <h2 class="text-xl text-center">
                  Phasollus risus turpis sit arnot magna non
                </h2>
              </div>
            </div>
          </div>
          <div class="flex justify-center 2xl:py-36 md:py-24">
            <div class="">
              <img
                src="./assets/img/3697355.jpg"
                alt=""
                class="xl:h-56 lg:h-44 h-36 ml-20 rounded-3xl xl:ml-20 md:ml-14 object-cover"
              />
              <div class="pt-3">
                <h1 class="text-2xl text-center font-bold">
                  Fast Home Delivery
                </h1>
                <h2 class="text-xl text-center">
                  Phasollus risus turpis sit arnot magna non.
                </h2>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div>
      <!-- menu -->
      <div class="md:grid md:grid-cols-2 h-screen">
        <div class="flex justify-center 2xl:ml-0 md:ml-20">
          <div>
            <h1
              class="2xl:text-5xl md:text-4xl font-extrabold md:pt-56 pt-11 text-center text-3xl"
            >
              Menu That Always <br />
              Make You Fall In Love
            </h1>
            <div class="md:py-3 md:text-start text-center">
              <button
                class="bg-black md:px-36 px-10 py-3 text-left rounded-xl text-lg text-white"
              >
                <span class="bg-yellow-500 px-2 rounded-full mr-4">1</span>
                Burger
              </button>
            </div>
            <div class="md:py-3 md:text-start text-center">
              <button
                class="bg-black md:px-36 px-10 py-3 text-left rounded-xl text-lg text-white"
              >
                <span class="bg-yellow-500 px-2 rounded-full mr-4">1</span>
                Pizza
              </button>
            </div>
            <div class="md:py-3 md:text-start text-center">
              <button
                class="bg-black md:px-36 px-10 py-3 text-left rounded-xl text-lg text-white"
              >
                <span class="bg-yellow-500 px-2 rounded-full mr-4">1</span
                >Cupcake
              </button>
            </div>
          </div>
        </div>
        <div>
          <div class="relative">
            <div
              class="bg-yellow-500 2xl:w-96 absolute translate-y-40 translate-x-16 rounded-2xl rotate-45 -z-10 shadow-2xl"
              style="height: 40rem"
            ></div>
          </div>
          <div class="md:pt-48">
            <img
              :src="images[currentImageIndex]"
              alt=""
              class="lg:h-96 lg:w-96 md:h-96 md:w-96 h-60 w-60 ml-28 object-cover"
            />
            <div class="relative">
              <div
                class="absolute z-20 2xl:left-48 xl:left-32 md:-translate-x-20 xl:translate-x-96 xl:translate-y-14 text-5xl left-24"
              >
                <button
                  @click="prevImage"
                  class="mr-10 border border-yellow-500 rounded-full px-7 py-7 relative"
                >
                  <p class="absolute -translate-x-4 -translate-y-7">&lt;</p>
                </button>
                <button
                  @click="nextImage"
                  class="mr-10 bg-yellow-500 text-white rounded-full px-7 py-7 relative"
                >
                  <p class="absolute -translate-x-4 -translate-y-7">&gt;</p>
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- update -->
    <div class="md:h-screen" style="margin-top: -3%">
      <div class="text-center text-5xl md:pt-5 font-bold">
        Our Popular Update <br />
        New Foods
      </div>
      <div class="text-center text-2xl font-medium text-slate-500 py-10">
        Maintain your dishes from everywhere. Add new dishes, upload photos,
        adapt
      </div>

      <div
        class="md:grid md:grid-cols-3 2xl:gap-24 2xl:px-72 xl:gap-9 md:gap-5 md:px-0 gap-5 px-11"
      >
        <div class="border p-3 mg:mb-0 mb-5">
          <div>
            <img
              src="./assets/img/dietary-salad-with-chicken-avocado-cucumber-tomato-chinese-cabbage.jpg"
              alt=""
              class="xl:h-80 lg:h-56 object-cover"
            />
          </div>
          <div>⭐⭐⭐⭐</div>
          <div class="text-2xl font-semibold lg:py-4 py-2">
            Humbugger Veggie
          </div>
          <div>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero
            dolorum iste voluptas odio, necessitatibus esse!
          </div>
          <div class="flex justify-between pt-10 self-end">
            <div class="text-2xl font-semibold">$5.80</div>
            <button class="bg-yellow-400 px-2 rounded-md">❤️</button>
          </div>
        </div>
        <div class="border p-3 mg:mb-0 mb-5 shadow-xl">
          <div>
            <img
              src="./assets/img/tom-yum-kung-thai-hot-spicy-soup-shrimp-with-lemon-grass-lemon-galangal-chilli-wooden-table-thailand-food.jpg"
              alt=""
              class="xl:h-80 lg:h-56 object-cover"
            />
          </div>
          <div>⭐⭐⭐⭐</div>
          <div class="text-2xl font-semibold mg:mb-0 mb-5 lg:py-4 py-2">
            Humbugger Veggie
          </div>
          <div>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero
            dolorum iste voluptas odio, necessitatibus esse!
          </div>
          <div class="flex justify-between pt-10 self-end">
            <div class="text-2xl font-semibold">$5.80</div>
            <button class="bg-yellow-400 px-2 rounded-md">❤️</button>
          </div>
        </div>
        <div class="border p-3">
          <div>
            <img
              src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg"
              alt=""
              class="xl:h-80 lg:h-56 object-cover"
            />
          </div>
          <div>⭐⭐⭐⭐</div>
          <div class="text-2xl font-semibold lg:py-4 py-2">
            Humbugger Veggie
          </div>
          <div>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero
            dolorum iste voluptas odio, necessitatibus esse!
          </div>
          <div class="flex justify-between pt-10 self-end">
            <div class="text-2xl font-semibold">$5.80</div>
            <button class="bg-yellow-400 px-2 rounded-md">❤️</button>
          </div>
        </div>
      </div>
    </div>

    <div class="h-screen bg-slate-100 overflow-hidden" id="">
      <div class="text-center" style="margin-top: 2%">
        <div class="text-5xl font-bold pt-10">Our Customer Services</div>
        <div class="text-2xl 2xl:pt-10">
          Maintain your dishes from everywhere. Add new dishes,upload photos,
          adapt
        </div>
      </div>
      <div class="h-4/5 relative md:block hidden">
        <div
          class="absolute w-2/12 xl:h-2/3 -rotate-45 2xl:translate-x-96 xl:translate-x-40 xl:left-96 xl:top-32 lg:left-48 md:top-56 md:left-14 rounded-3xl bg-yellow-500"
        >
          <div class="relative rotate-45">
            <div
              class="bg-white w-64 rounded-2xl h-52 shadow-2xl absolute -translate-y-28"
            >
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center pl-20">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="rounded-full h-28 w-28 border-8 border-white shadow-2xl object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
              <div></div>
              <div></div>
            </div>
            <div
              class="bg-white w-64 rounded-2xl h-52 shadow-2xl absolute translate-y-56 translate-x-4"
            >
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center pl-20">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="rounded-full h-28 w-28 border-8 border-white shadow-2xl object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
              <div></div>
              <div></div>
            </div>
            <div
              class="bg-white w-64 rounded-2xl h-52 shadow-2xl absolute top-40 left-96"
            >
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center pl-20">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="rounded-full h-28 w-28 border-8 border-white shadow-2xl object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
              <div></div>
              <div></div>
            </div>
            <div
              class="bg-white w-64 rounded-2xl h-52 shadow-2xl absolute -top-40 left-96"
            >
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center pl-20">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="rounded-full h-28 w-28 border-8 border-white shadow-2xl object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
              <div></div>
              <div></div>
            </div>
          </div>
        </div>
      </div>
      <div class="block md:hidden">
        <div class="grid grid-cols-2 grid-rows-2 gap-1 pt-28 px-2">
          <div>
            <div class="bg-white rounded-2xl">
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="h-20 rounded-full w-20 border-8 border-white object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div>
            <div class="bg-white rounded-2xl">
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="h-20 rounded-full w-20 border-8 border-white object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div>
            <div class="bg-white rounded-2xl">
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="h-20 rounded-full w-20 border-8 border-white object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div>
            <div class="bg-white rounded-2xl">
              <div class="-translate-y-10 px-4">
                <div class="flex justify-center">
                  <img
                    src="./assets/img/spaghetti-with-spicy-mixed-seafood-dark-background.jpg "
                    alt=""
                    class="h-20 rounded-full w-20 border-8 border-white object-cover"
                  />
                </div>
                <div class="pt-4">
                  <div class="text-xl font-bold">Mushroom Pizza</div>
                  <div class="py-2">⭐⭐⭐</div>
                  <div class="flex justify-between">
                    <div class="text-xl font-bold">7.56</div>
                    <button
                      class="text-xl font-bold bg-yellow-400 px-2 pb-1 rounded-full shadow-2xl"
                    >
                      +
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="md:h-screen bg-slate-50 overflow-hidden">
      <div class="text-center">
        <div class="text-6xl font-bold md:pt-20 pt-5" id="price">Pricing</div>
        <div class="text-2xl font-semibold text-slate-600 pt-10">
          Palladian yore dishes from everywhere. Add ne dishes
        </div>
      </div>
      <div>
        <div>
          <div class="relative" id="box">
            <div
              class="h-56 w-48 bg-yellow-500 absolute rounded-2xl rotate-12 2xl:left-1/4 xl:left-44 lg:translate-x-36 translate-y-20 z-20 md:block hidden"
            ></div>
            <div
              class="w-64 bg-yellow-500 absolute rounded-2xl rotate-45 left-2/4 translate-x-36 top-40 md:block hidden"
              style="height: 30rem"
            ></div>
          </div>
        </div>
        <div class="md:grid md:grid-cols-2 md:gap-10 2xl:px-96 md:pt-32 pt-10">
          <div class="flex md:justify-end justify-center z-50 md:pb-0 pb-10">
            <div class="bg-white px-10 py-8 shadow-2xl rounded-2xl">
              <div class="text-3xl font-medium">Free</div>
              <div class="text-md text-slate-400 font-medium">
                1 month for free
              </div>
              <div class="text-4xl font-semibold py-4">$0</div>
              <div class="font-semibold text-slate-500">
                <div class="pb-3">No actuation tees</div>
                <div class="pb-3">No hidden cousts ti</div>
                <div class="pb-3">Unlinked orders included</div>
                <div class="pb-3">(Fair use) = Only Smartphone</div>
              </div>
              <div class="text-center pt-10">
                <button
                  class="bg-slate-200 font-semibold rounded-2xl px-10 py-2 text-red-500"
                >
                  Get Started
                </button>
              </div>
            </div>
          </div>
          <div class="flex md:justify-start justify-center">
            <div class="flex justify-end z-50">
              <div class="bg-black px-10 py-8 shadow-2xl rounded-2xl">
                <div class="text-3xl font-medium text-white">Free</div>
                <div class="text-md text-slate-400 font-medium">
                  1 month for free
                </div>
                <div class="text-4xl font-semibold py-4 text-white">$50</div>
                <div class="font-semibold text-slate-500">
                  <div class="pb-3">No actuation tees</div>
                  <div class="pb-3">No hidden cousts ti</div>
                  <div class="pb-3">Unlinked orders included</div>
                  <div class="pb-3">(Fair use) = Only Smartphone</div>
                </div>
                <div class="text-center pt-10">
                  <button
                    class="text-white font-semibold rounded-2xl px-10 py-2 bg-red-500"
                  >
                    Get Started
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="h-screen overflow-hidden space-y-10 mt-10" id="aa">
      <div>
        <div class="flex justify-center">
          <div
            class="bg-zinc-800 text-center md:rounded-3xl py-10 lg:px-36 md:px-20 px-10"
          >
            <div class="text-white 2xl:text-5xl font-bold md:text-2xl">
              Discover Restaurants <br class="hidden md:block" />
              Near From you
            </div>
            <div
              class="flex justify-between items-center 2xl:px-32 2xl:gap-40 gap-10"
            >
              <div>
                <img
                  src="./assets/img/tom-yum-kung-thai-hot-spicy-soup-shrimp-with-lemon-grass-lemon-galangal-chilli-wooden-table-thailand-food.jpg"
                  alt=""
                  class="2xl:w-52 2xl:h-52 md:w-24 md:h-24 w-12 h-12 object-cover rounded-full"
                />
              </div>
              <div>
                <button
                  class="text-white md:font-extrabold bg-yellow-500 md:px-10 md:py-4 py-1 px-3 rounded-full"
                >
                  Explore now
                </button>
              </div>
              <div>
                <img
                  src="./assets/img/tom-yum-kung-thai-hot-spicy-soup-shrimp-with-lemon-grass-lemon-galangal-chilli-wooden-table-thailand-food.jpg"
                  alt=""
                  class="2xl:w-52 2xl:h-52 md:w-24 md:h-24 w-12 h-12 object-cover rounded-full"
                />
              </div>
            </div>
          </div>
        </div>
      </div>

      <div
        class="bg-black text-white"
        style="padding-bottom: 2rem; padding-top: 1rem"
      >
        <div
          class="grid md:grid-cols-4 md:grid-rows-1 grid-cols-2 grid-rows-2 xl:px-72 px-12 py-32 xl:gap-0 gap-10"
        >
          <div>
            <div class="pb-4 text-xl font-extrabold">
              Food <span class="text-yellow-500">.</span>
            </div>
            <div class="pb-4">
              Power u your business with out best digital marketing services
            </div>
            <div class="pb-4">
              <a href="#">f</a>
              <a href="#">x</a>
              <a href="#">in</a>
            </div>
          </div>
          <div class="">
            <div class="pb-2">
              <a href="#" class="font-bold">Menu </a>
            </div>
            <div class="pb-2">
              <a href="#">Home </a>
            </div>
            <div class="pb-2">
              <a href="#">Services </a>
            </div>
            <div class="pb-2">
              <a href="#">Pricing </a>
            </div>
            <div class="pb-2">
              <a href="#">Portfolio</a>
            </div>
          </div>
          <div>
            <div class="pb-2">
              <a href="#" class="font-bold">Contact us </a>
            </div>
            <div class="pb-2">
              <a href="#">Digimar.co</a>
            </div>
            <div class="pb-2">
              <a href="#">(323) 9435</a>
            </div>
            <div class="pb-2">
              <a href="#">Tegal, Indonesia</a>
            </div>
          </div>
          <div>
            <div class="pb-2">
              <a href="#" class="font-bold">Social Media</a>
            </div>
            <div class="pb-2">
              <a href="#">Facebook</a>
            </div>
            <div class="pb-2">
              <a href="#">Twitter</a>
            </div>
            <div class="pb-2">
              <a href="#">Instagram</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navshow: false,
      currentImageIndex: 0,
      images: [
        "https://cdn.pixabay.com/photo/2024/04/27/12/41/ai-generated-8723664_1280.png",
        "https://cdn.pixabay.com/photo/2017/12/05/20/10/pizza-3000285_960_720.png",
        "https://cdn.pixabay.com/photo/2017/09/07/11/25/cupcake-2724786_1280.png",
      ],
    };
  },
  methods: {
    nextImage() {
      this.currentImageIndex =
        (this.currentImageIndex + 1) % this.images.length;
    },
    prevImage() {
      this.currentImageIndex =
        (this.currentImageIndex - 1 + this.images.length) % this.images.length;
    },
  },
};
</script>
<style>
.slide-fade-enter-active {
  transition: all 0.1s ease-in-out;
}

.slide-fade-leave-active {
  transition: all 0.3s ease-in-out;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateY(-20px);
  opacity: 0;
}
</style>
