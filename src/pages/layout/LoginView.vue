<template>
    <div class="bg-white min-h-screen" style="zoom: 0.77">
      <div class="w-36 h-24 ml-12 mt-2">
        <router-link to="/">
            <img src="../../assets/Logo1.png" alt="Logo">
        </router-link>
      </div>

      <div class="pt-16 pb-12 px-12 mx-auto mt-6 border-1.5 border-achmi-login rounded-2xl w-1/3">
        <p class="font-montserrat font-medium text-2xl text-black">Log in to Achmitech</p>

        <div class="pt-14">
            <p class="mb-1 font-montserrat font-normal text-black text-sm text-left">Email Address</p>
            <div class="pb-2">
                <input type="email" class="rounded-md border-1.5 border-achmi-login py-3 w-full font-montserrat text-sm tracking-widest pl-10 pr-20" :class="{ 'placeholder-active': isPlaceholderActive }" v-model="inputValue" @focus="handleFocus" @blur="handleBlur">
            </div>

            <div class="relative my-10">
                <p class="absolute left-0 bottom-1 font-montserrat font-normal text-black text-sm inline-block text-left">Password</p>
                <p class="absolute right-0 bottom-1 font-montserrat font-semibold text-achmi-primary text-xs inline text-right">Forgot Password ?</p>        
            </div>
            <div class="relative">
                <input type="password" class="border-1.5 border-achmi-login inline-block rounded-md py-3 w-full font-montserrat text-sm tracking-widest pl-10 pr-5" :class="{ 'placeholder-active': isPlaceholderActiveP }" v-model="inputValueP" @focus="handleFocusP" @blur="handleBlurP">
            </div>
        </div>

        <router-link to="/HomeCandidat"><button class="rounded-full bg-achmi-primary text-white font-montserrat text-lg font-medium mt-12 py-2.5 w-full">Login</button></router-link>
        
        <div class="mt-16 mb-9">
          <div class="relative">
            <p class="absolute inset-x-0 -mt-3 z-10">Don’t have an Achmitech account?</p>
            <div class="bg-black h-2023 w-full"></div>
            <div class="h-2 -mt-1 bg-white border-none mx-auto w-8/12 absolute inset-0"></div>
          </div>
        </div>
        <router-link to="/signup">
          <button class="rounded-full bg-achmi-secondary text-white font-montserrat text-lg font-medium w-full py-2.5">Sign Up</button>
        </router-link>
        </div>
      
     
    </div>
</template>

<script>
import { ref, computed } from 'vue'
export default {
  setup(){
    const placeHolder = ref('e.g example@email.com')
    const placeHolderP = ref('Write your password')
    const inputValue = ref('e.g example@email.com')
    const inputValueP = ref('Write your password')


    const isPlaceholderActive = computed(() => {
      return inputValue.value === '' || inputValue.value === placeHolder.value;
    })

    const isPlaceholderActiveP = computed(() => {
      return inputValueP.value === '' || inputValueP.value === placeHolderP.value;
    })
    const handleFocus = () => {
      if(inputValue.value == placeHolder.value){
        inputValue.value = ''
      }
    }

    const handleBlur = () => {
      if(inputValue.value === ''){
        inputValue.value = placeHolder.value
      }
    }

    const handleFocusP = () => {
      if(inputValueP.value == placeHolderP.value){
        inputValueP.value = ''
      }
    }

    const handleBlurP = () => {
      if(inputValueP.value === ''){
        inputValueP.value = placeHolderP.value
      }
    }

    return {inputValue, placeHolder, handleFocus, handleBlur, isPlaceholderActive, inputValueP, placeHolderP, handleFocusP, handleBlurP, isPlaceholderActiveP}
  }
}
</script>