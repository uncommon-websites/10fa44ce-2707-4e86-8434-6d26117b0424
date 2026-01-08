<script lang="ts">
  import { base } from '$app/paths';
</script>

<section class="relative pt-20 pb-16 overflow-hidden bg-white">
  <div class="container mx-auto px-4 max-w-7xl">
    <div class="flex flex-col items-center text-center mb-12">
      <span class="text-blue-600 font-semibold tracking-wider text-xs uppercase mb-4">Workforce Operations Platform</span>
      <h1 class="text-5xl md:text-7xl font-bold tracking-tight text-gray-900 mb-8 max-w-4xl leading-tight">
        The first <span class="relative inline-block">training<svg class="absolute w-full h-3 -bottom-1 left-0 text-blue-200 -z-10" viewBox="0 0 100 10" preserveAspectRatio="none"><path d="M0 5 Q 50 10 100 5" stroke="currentColor" stroke-width="8" fill="none" /></svg></span> and <span class="relative inline-block">operations<svg class="absolute w-full h-3 -bottom-1 left-0 text-blue-200 -z-10" viewBox="0 0 100 10" preserveAspectRatio="none"><path d="M0 5 Q 50 10 100 5" stroke="currentColor" stroke-width="8" fill="none" /></svg></span> <br class="hidden md:block" /> platform your staff will love
      </h1>
      
      <button class="bg-black text-white px-6 py-3 rounded-full font-medium flex items-center gap-2 hover:bg-gray-800 transition-colors cursor-pointer">
        Book a demo
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
          <path stroke-linecap="round" stroke-linejoin="round" d="M4.5 19.5l15-15m0 0H8.25m11.25 0v11.25" />
        </svg>
      </button>
    </div>

    <div class="relative mt-12 mx-auto max-w-6xl">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 items-end">
        <!-- Left Image -->
        <div class="rounded-3xl overflow-hidden h-64 md:h-80 relative bg-gray-100">
           <img src="https://images.unsplash.com/photo-1556761175-5973dc0f32e7?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Staff working" class="w-full h-full object-cover" />
        </div>

        <!-- Center Phone -->
        <div class="relative z-10 -mt-12 md:-mt-24 text-center">
            <div class="relative mx-auto border-gray-800 bg-gray-800 border-[14px] rounded-[2.5rem] h-[500px] w-[280px] shadow-xl">
                <div class="h-[32px] w-[3px] bg-gray-800 absolute -start-[17px] top-[72px] rounded-s-lg"></div>
                <div class="h-[46px] w-[3px] bg-gray-800 absolute -start-[17px] top-[124px] rounded-s-lg"></div>
                <div class="h-[46px] w-[3px] bg-gray-800 absolute -start-[17px] top-[178px] rounded-s-lg"></div>
                <div class="h-[64px] w-[3px] bg-gray-800 absolute -end-[17px] top-[142px] rounded-e-lg"></div>
                <div class="rounded-[2rem] overflow-hidden w-full h-full bg-white relative">
                    <!-- Screen Content Mockup -->
                    <div class="bg-blue-600 text-white p-6 pt-12 rounded-b-3xl h-3/5 relative">
                         <div class="flex justify-between items-center mb-4">
                            <div class="w-8 h-8 bg-white/20 rounded-full"></div>
                            <div class="w-8 h-8 bg-white/20 rounded-full"></div>
                         </div>
                         <h3 class="text-2xl font-bold leading-tight mb-2">How do you advise guests at food options?</h3>
                         <div class="bg-white text-black p-3 rounded-xl mt-4 shadow-lg flex items-center gap-3">
                            <div class="w-6 h-6 rounded-full border border-gray-300"></div>
                            <span class="text-sm font-medium">Ask about preferences</span>
                         </div>
                         <div class="bg-white/20 text-white p-3 rounded-xl mt-2 flex items-center gap-3">
                            <div class="w-6 h-6 rounded-full border border-white/50"></div>
                            <span class="text-sm font-medium">Wait for them to ask</span>
                         </div>
                    </div>
                    <div class="p-4">
                         <div class="h-2 bg-gray-100 rounded w-3/4 mb-2"></div>
                         <div class="h-2 bg-gray-100 rounded w-1/2"></div>
                    </div>
                    <!-- Bottom Nav -->
                    <div class="absolute bottom-0 w-full border-t border-gray-100 p-4 flex justify-around">
                        <div class="w-6 h-6 bg-gray-200 rounded-full"></div>
                        <div class="w-6 h-6 bg-blue-600 rounded-full"></div>
                        <div class="w-6 h-6 bg-gray-200 rounded-full"></div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Right Image -->
        <div class="rounded-3xl overflow-hidden h-64 md:h-80 relative bg-gray-100">
            <img src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Team meeting" class="w-full h-full object-cover" />
             <!-- Floating badges -->
             <div class="absolute top-4 left-4 bg-white px-3 py-1.5 rounded-full shadow-md text-xs font-medium flex items-center gap-1">
                <span class="w-2 h-2 bg-orange-500 rounded-full"></span> Service Training
             </div>
             <div class="absolute bottom-12 right-4 bg-white px-3 py-1.5 rounded-full shadow-md text-xs font-medium flex items-center gap-1">
                <span class="w-2 h-2 bg-red-500 rounded-full"></span> Inventory Checklist
             </div>
        </div>
      </div>
    </div>

    <div class="text-center mt-12 max-w-2xl mx-auto">
        <p class="text-gray-600 text-lg">
            Employee training, checklists and communication all under one roof. Made for your deskless workforce. Gamified in one employee app.
        </p>
    </div>
  </div>
</section>
