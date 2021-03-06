<template>
  <div class="py-12 font-sans text-sm sm:text-base">
    <div class="mx-auto w-7/8 sm:w-10/12 md:w-11/12 md:px-12">
      <div class="flex flex-wrap justify-center">
        <!--  -->

        <!-- Column -->
        <div class="flex justify-center w-full px-2 py-2 my-1 xl:w-1/2 lg:my-4 lg:px-4 xl:px-2">
          <!-- Card 1 Starts -->
          <div class="scene scene--card zoom">
            <div
              class="card"
              @click="
                firstCard == undefined
                  ? (firstCard = 1)
                  : (firstCard = undefined)
              "
              :class="{ flipme: firstCard == 1 }"
            >
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--front hover:shadow-xl"
              >
                <div class="text-5xl font-semibold sm:text-6xl popout font-cardface">What is JS?</div>
              </div>
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--back hover:shadow-xl"
              >
                <div class="font-light popout">
                  <div class="px-10">
                    <div class="text-left">
                      <p>
                        "JavaScript (JS) is a lightweight, interpreted, or
                        just-in-time compiled programming language with
                        first-class functions. While it is most well-known as
                        the scripting language for Web pages, many non-browser
                        environments also use it, such as Node.js, Apache
                        CouchDB and Adobe Acrobat. JavaScript is a
                        prototype-based, multi-paradigm, single-threaded,
                        dynamic language, supporting object-oriented,
                        imperative, and declarative (e.g. functional
                        programming) styles."
                      </p>

                      <p class="ml-4 italic">
                        - excerpt from MDN docs. Click
                        <a
                          href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"
                          target="blank"
                          class="underline cursor-alias hover:text-basicred"
                        >here</a>
                        to read more
                      </p>
                      <br />
                      <ul class="list-disc list-inside">
                        <li>
                          You can learn more about the technical terms at
                          <a
                            href="https://en.wikipedia.org/wiki/JavaScript"
                            target="black"
                            class="underline cursor-alias hover:text-basicred"
                          >Wikepedia</a>
                        </li>
                        <li>
                          You can also find a quick JS intro at
                          <a
                            href="https://javascript.info/intro"
                            target="blank"
                            class="underline hover:text-basicred cursor-alias"
                          >javascript.info</a>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Card 1 Ends  -->
        </div>

        <!-- END Column -->
        <!-- Column -->
        <div class="flex justify-center w-full px-2 py-2 my-1 xl:w-1/2 lg:my-4 lg:px-4 xl:px-2">
          <!-- Card 2 Starts -->
          <div class="scene scene--card zoom">
            <div
              class="card"
              @click="
                secondCard == undefined
                  ? (secondCard = 1)
                  : (secondCard = undefined)
              "
              :class="{ flipme: secondCard == 1 }"
            >
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--front hover:shadow-xl"
              >
                <div
                  class="font-sans text-5xl font-semibold sm:text-6xl popout font-cardface"
                >Data Types</div>
              </div>
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--back hover:shadow-xl"
              >
                <div class="font-sans font-light popout">
                  <div class="px-10">
                    <h3
                      class="mb-2 font-sans text-xl font-normal uppercase sm:text-3xl"
                    >8 Data Types</h3>
                    <div class="text-left">
                      <ul>
                        <li class="font-normal underline">7 Primitive</li>
                        <ol class="pl-4 list-decimal list-inside">
                          <li>
                            <span class="mr-2 font-bold">Boolean:</span> True
                            and False
                          </li>
                          <li>
                            <span class="mr-2 font-bold">null:</span> a special
                            keyword denoting a null value
                          </li>
                          <li>
                            <span class="mr-2 font-bold">undefined:</span> A
                            top-level property whose value is not defined
                          </li>
                          <li>
                            <span class="mr-2 font-bold">Number:</span> An
                            integer or floating point number
                          </li>
                          <li>
                            <span class="mr-2 font-bold">BigInt:</span> An
                            integer with arbitrary precision
                          </li>
                          <li>
                            <span class="mr-2 font-bold">String:</span> A
                            sequence of characters that represent a text value
                          </li>
                          <li>
                            <span class="mr-2 font-bold">Symbol:</span> A data
                            type whose instances are unique and immutable
                          </li>
                        </ol>
                        <li>
                          <span class="font-bold">+ Object</span>
                          <!-- (see objects section for more details) -->
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Card 2 Ends  -->
        </div>

        <!-- END Column -->

        <!-- Column -->
        <div class="flex justify-center w-full px-2 py-2 my-1 xl:w-1/2 lg:my-4 lg:px-4 xl:px-2">
          <!-- Card 3 Starts -->
          <div class="scene scene--card zoom">
            <div
              class="card"
              @click="
                thirdCard == undefined
                  ? (thirdCard = 1)
                  : (thirdCard = undefined)
              "
              :class="{ flipme: thirdCard == 1 }"
            >
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--front hover:shadow-xl"
              >
                <div
                  class="font-sans text-5xl font-semibold sm:text-6xl popout font-cardface"
                >Variables</div>
              </div>
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--back hover:shadow-xl"
              >
                <div class="font-sans font-light popout">
                  <div class="px-10">
                    <div class="text-left">
                      <p class="font-semibold">Variables are containers that hold reusable data</p>
                      <p class="mt-3 underline">3 ways to declare (create) a variable:</p>
                      <ul class="ml-4">
                        <li>
                          <span class="mr-2 font-bold">var:</span>declares a
                          variable (
                          <strong>DON'T</strong> use this method)
                        </li>
                        <li>
                          <span class="mr-2 font-bold">let:</span>declares a
                          block-scoped, local variable
                        </li>
                        <li>
                          <span class="mr-2 font-bold">const:</span>declares a
                          block-scoped, read-only named constant
                        </li>
                      </ul>
                      <p class="mt-2 underline">Variable Assignment</p>
                      <p>
                        The declared variable is assigned data using the
                        assignment operator "=". The value of the assigned data
                        can be any of the following
                      </p>
                      <div class="w-3/4 mx-auto mt-2 sm:w-6/12">
                        <div class="flex justify-around w-full">
                          <div>
                            <ul class="list-disc">
                              <li>String</li>
                              <li>Number</li>
                              <li>Boolean</li>
                              <li>Null</li>
                            </ul>
                          </div>
                          <div>
                            <ul class="list-disc">
                              <li>Undefined</li>
                              <li>an Array</li>
                              <li>an Object</li>
                            </ul>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Card 3 Ends  -->
        </div>

        <!-- END Column -->
        <!-- Column -->
        <div class="flex justify-center w-full px-2 py-2 my-1 xl:w-1/2 lg:my-4 lg:px-4 xl:px-2">
          <!-- Card 4 Starts -->
          <div class="scene scene--card zoom">
            <div
              class="card"
              @click="
                fourthCard == undefined
                  ? (fourthCard = 1)
                  : (fourthCard = undefined)
              "
              :class="{ flipme: fourthCard == 1 }"
            >
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--front hover:shadow-xl"
              >
                <div
                  class="font-sans text-5xl font-semibold sm:text-6xl popout font-cardface"
                >Comments</div>
              </div>
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--back hover:shadow-xl"
              >
                <div class="font-sans font-light popout">
                  <div class="px-10">
                    <div class="mb-6 text-xl font-semibold sm:text-2xl">
                      <h3>2 Types of Comments</h3>
                    </div>
                    <div class="flex justify-center">
                      <img
                        src="../assets/comments.png"
                        alt="comments code
                      snippet"
                        class="w-auto h-48 rounded-lg"
                      />
                    </div>
                    <div class="w-11/12 mx-auto mt-6 text-left">
                      <ul class="list-disc">
                        <li>
                          Comments are treated like white space and they are
                          discarded when the script is executed
                        </li>
                        <li>
                          They can be used to leave notes or descriptions of
                          code and also to prevent a selection of code from
                          running
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Card 4 Ends  -->
        </div>

        <!-- END Column -->
        <!-- Column -->
        <div class="flex justify-center w-full px-2 py-2 my-1 xl:w-1/2 lg:my-4 lg:px-4 xl:px-2">
          <!-- Card 5 Starts -->
          <div class="scene scene--card zoom">
            <div
              class="card"
              @click="
                fifthCard == undefined
                  ? (fifthCard = 1)
                  : (fifthCard = undefined)
              "
              :class="{ flipme: fifthCard == 1 }"
            >
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--front hover:shadow-xl"
              >
                <div
                  class="font-sans text-5xl font-semibold sm:text-6xl popout font-cardface"
                >Operators</div>
              </div>
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--back hover:shadow-xl"
              >
                <div class="font-sans font-light popout">
                  <h3
                    class="mb-4 text-lg font-semibold sm:text-xl"
                  >Click the buttons to see the Operators</h3>
                  <div class="px-10">
                    <div class="mb-6 text-xl font-semibold">
                      <div
                        class="flex flex-col items-center justify-center w-7/12 mx-auto sm:w-2/4"
                      >
                        <button
                          class="w-full px-2 py-1 mb-4 font-semibold uppercase border-2 border-solid rounded shadow-lg border-basicdark hover:bg-basicdark hover:text-basiclight"
                          @click.stop="showArrith = true"
                        >Arithmetic</button>
                        <button
                          class="w-full px-2 py-1 mb-4 font-semibold uppercase border-2 border-solid rounded shadow-lg border-basicdark hover:bg-basicdark hover:text-basiclight"
                          @click.stop="showAssign = true"
                        >Assignment</button>
                        <button
                          class="w-full px-2 py-1 mb-4 font-semibold uppercase border-2 border-solid rounded shadow-lg border-basicdark hover:bg-basicdark hover:text-basiclight"
                          @click.stop="showCompar = true"
                        >Comparison</button>
                        <button
                          class="w-full px-2 py-1 mb-4 font-semibold uppercase border-2 border-solid rounded shadow-lg border-basicdark hover:bg-basicdark hover:text-basiclight"
                          @click.stop="showLogical = true"
                        >Logical</button>
                        <button
                          class="w-full px-2 py-1 font-semibold uppercase border-2 border-solid rounded shadow-lg border-basicdark hover:bg-basicdark hover:text-basiclight"
                          @click.stop="showType = true"
                        >type</button>
                      </div>
                    </div>
                    <p class="pb-2">
                      Check out the
                      <a
                        href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Bitwise_Operators"
                        target="blank "
                        class="underline hover:text-basicred cursor-alias"
                      >MDN Docs</a>
                      for info on Bitwise Operators
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Card 5 Ends  -->
        </div>

        <!-- END Column -->

        <!-- Column -->
        <div class="flex justify-center w-full px-2 py-2 my-1 xl:w-1/2 lg:my-4 lg:px-4 xl:px-2">
          <!-- Card 6 Starts -->
          <div class="scene scene--card zoom">
            <div
              class="card"
              @click="
                sixthCard == undefined
                  ? (sixthCard = 1)
                  : (sixthCard = undefined)
              "
              :class="{ flipme: sixthCard == 1 }"
            >
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--front hover:shadow-xl"
              >
                <div
                  class="font-sans text-5xl font-semibold sm:text-6xl popout font-cardface"
                >Strict Mode</div>
              </div>
              <div
                class="flex items-center justify-center rounded-lg shadow-lg card__face card__face--back hover:shadow-xl"
              >
                <div class="font-sans font-light popout">
                  <div class="px-10 text-left">
                    <p class="font-semibold">What is Strict Mode?</p>
                    <p
                      class="mb-3"
                    >Strict mode allows you to place a program or function in a 'strict' operating context</p>
                    <p class="font-semibold">Declaring Strict Mode</p>
                    <p
                      class="mb-3"
                    >Add the "use strict" directive at the top of a script or a function</p>
                    <p class="mb-1 font-semibold">Changes/Benefits of Strict Mode</p>
                    <ol class="list-decimal list-inside">
                      <li>Eliminates some JavaScript silent errors by changing them to throw errors</li>
                      <li>Fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that's not strict mode</li>
                      <li>Prohibits some syntax likely to be defined in future versions of ECMAScript</li>
                    </ol>
                    <p class="ml-4 italic">
                      - excerpt from MDN docs. Click
                      <a
                        href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode"
                        target="blank"
                        class="underline cursor-alias hover:text-basicred"
                      >here</a>
                      to read more
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Card 6 Ends  -->
        </div>

        <!-- END Column -->
      </div>
    </div>
    <!-- <div @mouseover="modalPlease" @mouseleave="modalPlease"></div> -->
    <app-modal
      v-if="showArrith"
      @close="showArrith = false"
      backgroundColor="bg-basiclight"
      textColor="text-basicdark"
      buttonColor="bg-basiclight hover:text-basiclight hover:bg-basicdark border-basicdark"
    >
      <template v-slot:header>
        <h3 class="text-xl uppercase">Arithmetic Operators</h3>
      </template>
      <template v-slot:body>
        <arith-operators></arith-operators>
      </template>
    </app-modal>
    <app-modal
      v-if="showAssign"
      @close="showAssign = false"
      backgroundColor="bg-basiclight"
      textColor="text-basicdark"
      buttonColor="bg-basiclight hover:text-basiclight hover:bg-basicdark border-basicdark"
    >
      <template v-slot:header>
        <h3 class="text-xl uppercase">Assignment Operators</h3>
      </template>
      <template v-slot:body>
        <assign-operators></assign-operators>
      </template>
    </app-modal>
    <app-modal
      v-if="showCompar"
      @close="showCompar = false"
      backgroundColor="bg-basiclight"
      textColor="text-basicdark"
      buttonColor="bg-basiclight hover:text-basiclight hover:bg-basicdark border-basicdark"
    >
      <template v-slot:header>
        <h3 class="text-xl uppercase">Comparison Operators</h3>
      </template>
      <template v-slot:body>
        <compar-operators></compar-operators>
      </template>
    </app-modal>
    <app-modal
      v-if="showLogical"
      @close="showLogical = false"
      backgroundColor="bg-basiclight"
      textColor="text-basicdark"
      buttonColor="bg-basiclight hover:text-basiclight hover:bg-basicdark border-basicdark"
    >
      <template v-slot:header>
        <h3 class="text-xl uppercase">Logical Operators</h3>
      </template>
      <template v-slot:body>
        <logical-operators></logical-operators>
      </template>
    </app-modal>
    <app-modal
      v-if="showType"
      @close="showType = false"
      backgroundColor="bg-basiclight"
      textColor="text-basicdark"
      buttonColor="bg-basiclight hover:text-basiclight hover:bg-basicdark border-basicdark"
    >
      <template v-slot:header>
        <h3 class="text-xl uppercase">Type Operators</h3>
      </template>
      <template v-slot:body>
        <type-operators></type-operators>
      </template>
    </app-modal>
    <div class="mt-10 text-center">
      <a href="#top" class="text-xl underline uppercase text-basicdark">
        <button
          class="px-5 py-2 font-semibold uppercase border-2 border-solid rounded shadow-lg border-basicdark hover:bg-basicdark hover:text-basiclight bg-basiclight xl:hidden"
        >Back to Top</button>
      </a>
    </div>
  </div>
</template>

<script>
import AppModal from "../components/AppModal";
import ArithOperators from "../components/modal-contents/basics/ArithOperators";
import AssignOperators from "../components/modal-contents/basics/AssignOperators";
import ComparOperators from "../components/modal-contents/basics/ComparOperators";
import LogicalOperators from "../components/modal-contents/basics/LogicalOperators";
import TypeOperators from "../components/modal-contents/basics/TypeOperators";
export default {
  components: {
    AppModal,
    ArithOperators,
    AssignOperators,
    ComparOperators,
    LogicalOperators,
    TypeOperators
  },
  data() {
    return {
      firstCard: undefined,
      secondCard: undefined,
      thirdCard: undefined,
      fourthCard: undefined,
      fifthCard: undefined,
      sixthCard: undefined,
      showArrith: false,
      showAssign: false,
      showCompar: false,
      showLogical: false,
      showType: false,
      hoverButton: false
    };
  }
};
</script>
<style scoped>
.scene {
  perspective: 1200px;
  height: 450px;
  width: 500px;
}

.card {
  width: 100%;
  height: 100%;
  transition: transform 1s;
  transform-style: preserve-3d;
  cursor: pointer;
  position: relative;
  transform-origin: center right;
}

.flipme {
  transform: translateX(-100%) rotateY(-180deg);
}

.card__face {
  position: absolute;
  width: 100%;
  height: 100%;
  color: hsl(352.2, 84%, 20%);
  text-align: center;
  transform-style: preserve-3d;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

.card__face--front {
  background: hsl(352.2, 84.3%, 95%);
}

.card__face--back {
  background: hsl(352.2, 84.3%, 95%);
  transform: rotateY(180deg);
  color: hsl(352.2, 84%, 20%);
}

.popout {
  transform: translateZ(100px);
}
</style>
