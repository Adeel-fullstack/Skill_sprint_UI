
<template>
  <nav class="bg-[#F8FAFC] px-3 md:px-8 ">
    
    <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-3 items-center gap-3">
      
      <!-- Logo -->
      <div class="flex justify-center md:justify-end">
        <img 
          src="/navlogo.png" 
          alt="Skill Sprint Robot" 
          class="w-[100px] md:w-[130px] h-auto"
        />
      </div>
      
      <!-- Menu -->
      <div class="flex justify-center">
        <div class="flex flex-nowrap justify-center items-center gap-3 md:gap-6
                    bg-gray-200 px-4 md:px-8 py-2 md:py-4 
                    rounded-full text-xs md:text-sm font-medium text-gray-500">
          
         <router-link  to="/" class="text-blue-600 cursor-pointer transition">Home</router-link>
        <a href ="#" class="text-gray-500 hover:text-blue-600 cursor-pointer transition">Community</a>
        <a href ="#" class="text-gray-500 hover:text-blue-600 cursor-pointer transition">  Sprints</a>
        <a href ="#" class="text-gray-500 hover:text-blue-600 cursor-pointer transition">  Team</a>
         <router-link to="/AboutUs" class="text-gray-500 hover:text-blue-600 cursor-pointer transition">About Us </router-link>


        </div>
      </div>

      <!-- Button -->
      <div class="flex justify-center md:justify-start">
        <button class="bg-blue-600 text-white px-3 md:px-7 py-2 md:py-4 
                       text-xs md:text-sm rounded-full font-medium 
                       hover:bg-blue-700 transition shadow-sm shadow-blue-100">
          Join the Sprint
        </button>
      </div>

    </div>

  </nav>
</template>

