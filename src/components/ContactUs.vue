<template>
  <div class="min-h-screen bg-[#F8FAFC] flex flex-col items-center p-4 md:p-8 space-y-12">
    
    <div class="max-w-6xl w-full  bg-[#E8F2FF] rounded-xl  overflow-hidden p-5 flex flex-col md:flex-row">
      <div class="bg-[#007bff] w-full md:w-2/5 p-8 md:p-12 rounded-xl text-white flex flex-col justify-between">
        <div>
          <p class="tracking-widest text-xs font-semibold mb-4 opacity-90 uppercase">Contact Us</p>
          <h1 class="text-4xl md:text-5xl font-bold leading-tight mb-6">
            Let's Build <br /> Something <br /> Together
          </h1>
          <p class="text-lg opacity-90 max-w-xs">
            Have an idea, partnership proposal, or question? Send it our way and let's sprint on it.
          </p>
        </div>

        <div class="mt-12 space-y-6">
          <div class="flex items-center gap-4">
            <div class="bg-black p-3 rounded-lg">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
              </svg>
            </div>
            <div>
              <p class="text-sm font-bold">Email</p>
              <p class="text-sm opacity-80">skillsprint@gmail.com</p>
            </div>
          </div>

          <div class="flex items-center gap-4">
            <div class="bg-black p-3 rounded-lg">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
              </svg>
            </div>
            <div>
              <p class="text-sm font-bold">Phone</p>
              <p class="text-sm opacity-80">+92 317 444 4441</p>
            </div>
          </div>
        </div>
      </div>

      <div class="w-full  bg-[#E8F2FF] md:w-3/5 p-8 md:p-12">
        <form @submit.prevent="handleSubmit" class="space-y-6">
          <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
            <div class="space-y-2">
              <label class="block text-sm font-bold">Full Name</label>
              <input 
                type="text" 
                placeholder="Enter your name" 
                class="w-full px-4 py-3 rounded-xl bg-white focus:ring-2 focus:ring-[#007bff] outline-none transition border border-gray-100"
              />
            </div>
            <div class="space-y-2">
              <label class="block text-sm font-bold text-gray-700">Email Address</label>
              <input 
                type="email" 
                placeholder="Enter your email" 
                class="w-full px-4 py-3 rounded-xl bg-white focus:ring-2 focus:ring-[#007bff] outline-none transition border border-gray-100"
              />
            </div>
          </div>

          <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
            <div class="space-y-2">
              <label class="block text-sm font-bold text-gray-700">Phone Number</label>
              <div class="relative">
                <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none">
                  <span class="text-sm text-gray-500">🇵🇰 PK +92</span>
                </div>
                <input 
                  type="tel" 
                  placeholder="300-0000000" 
                  class="w-full pl-20 pr-4 py-3 rounded-xl border bg-white border-gray-200 focus:ring-2 focus:ring-[#007bff] outline-none transition"
                />
              </div>
            </div>
            <div class="space-y-2">
              <label class="block text-sm font-bold text-gray-700">University / Organization</label>
              <input 
                type="text" 
                placeholder="Enter organization" 
                class="w-full px-4 py-3 rounded-xl border border-gray-200 bg-white focus:ring-2 focus:ring-[#007bff] outline-none transition"
              />
            </div>
          </div>

          <div class="space-y-2">
            <label class="block text-sm font-bold text-gray-700">Purpose of Contact</label>
            <select class="w-full px-4 py-3 rounded-xl border border-gray-200 bg-white focus:ring-2 focus:ring-[#007bff] outline-none transition">
              <option disabled selected>Select Purpose</option>
              <option>Partnership</option>
              <option>General Inquiry</option>
              <option>Technical Support</option>
            </select>
          </div>

          <div class="space-y-2">
            <label class="block text-sm font-bold text-gray-700">Messages</label>
            <textarea 
              rows="4" 
              class="w-full px-4 py-3 rounded-xl border border-gray-200 bg-white focus:ring-2 focus:ring-[#007bff] outline-none transition resize-none"
            ></textarea>
          </div>

          <div class="flex items-center gap-3">
            <input type="checkbox" id="privacy" class="w-5 h-5 rounded border-gray-300 text-[#007bff]" />
            <label for="privacy" class="text-sm text-gray-600">
              You agree to our friendly <a href="#" class="text-[#007bff] underline">privacy policy</a>.
            </label>
          </div>

          <button type="submit" class="bg-[#007bff] hover:bg-[#0069d9] text-white font-bold py-3 px-10 rounded-xl transition-all active:scale-95 shadow-lg shadow-blue-200">
            Send Message
          </button>
        </form>
      </div>
    </div>

    <div class="w-full max-w-6xl mt-10 px-10 py-6 bg-[#E8F2FF] rounded-[30px] flex flex-col md:flex-row items-center justify-between gap-12 md:gap-24 shadow-sm border-3 border-white">
  <div class="flex items-center gap-0"> <div class="text-[#1D7CFF]">
      <img 
        src="/sidelogo.png"
        class="w-[120px] md:w-[180px] h-auto" 
        alt="Logo"
      />
    </div>
    <h1 class="text-[#1D7CFF] text-5xl md:text-4xl font-bold leading-tight max-w-[300px]">
      Backed by <br /> Real Numbers
    </h1>
  </div>

  <div class="flex flex-wrap justify-center gap-10 md:gap-20">
    <div class="flex flex-col">
      <span class="text-[#1D7CFF] text-3xl font-bold">1,000+</span>
      <span class="text-[#111827] text-xl font-bold mt-1">Students</span>
      <span class="text-gray-500 text-[10px] font-semibold uppercase tracking-widest mt-1">Squad Expanding</span>
    </div>
    
    <div class="flex flex-col">
      <span class="text-[#1D7CFF] text-3xl font-bold">20+</span>
      <span class="text-[#111827] text-xl font-bold mt-1">Universities</span>
      <span class="text-gray-500 text-[10px] font-semibold uppercase tracking-widest mt-1">Campus Approved</span>
    </div>
    
    <div class="flex flex-col">
      <span class="text-[#1D7CFF] text-3xl font-bold">10+</span>
      <span class="text-[#111827] text-xl font-bold mt-1">Mentors</span>
      <span class="text-gray-500 text-[10px] font-semibold uppercase tracking-widest mt-1">Grownups Who Help</span>
    </div>
  </div>
</div>

  </div>
</template>

<script setup>
const handleSubmit = () => {
  console.log('Form submitted!');
};
</script>

<style scoped>
h2 {
  letter-spacing: -0.02em;
}
</style>