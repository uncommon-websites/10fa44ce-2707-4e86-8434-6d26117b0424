<section class="py-20 bg-white">
    <div class="container mx-auto px-4 max-w-6xl">
        <div class="text-center mb-12">
            <span class="text-blue-500 font-semibold tracking-wider text-xs uppercase mb-4 block">Empowering Frontline Workers</span>
            <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">
                Boost employee performance.<br />
                Achieve operational excellence.
            </h2>
            <p class="text-gray-600 text-lg max-w-2xl mx-auto mb-8">
                One platform that ties it all together. Train teams, guide daily work, stay compliant, and keep everyone aligned.
            </p>
            <div class="flex justify-center gap-4">
                <button class="bg-blue-600 text-white px-6 py-2.5 rounded-full font-medium hover:bg-blue-700 transition-colors">
                    Book a demo <span class="ml-1">↗</span>
                </button>
                <button class="text-gray-900 px-6 py-2.5 rounded-full font-medium hover:bg-gray-50 transition-colors flex items-center gap-1">
                    Explore product <span class="text-gray-400">›</span>
                </button>
            </div>
        </div>

        <!-- Video/Image Container -->
        <div class="relative rounded-3xl overflow-hidden shadow-2xl bg-gray-900 aspect-video md:aspect-[21/9] group cursor-pointer">
            <img src="https://images.unsplash.com/photo-1600880292203-757bb62b4baf?ixlib=rb-4.0.3&auto=format&fit=crop&w=1600&q=80" alt="Worker using app" class="w-full h-full object-cover opacity-80 group-hover:opacity-60 transition-opacity" />
            
            <div class="absolute inset-0 flex items-center justify-center">
                <div class="w-16 h-16 bg-white/20 backdrop-blur-sm rounded-full flex items-center justify-center group-hover:scale-110 transition-transform">
                    <div class="w-12 h-12 bg-white rounded-full flex items-center justify-center pl-1">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-6 h-6 text-blue-600">
                            <path fill-rule="evenodd" d="M4.5 5.653c0-1.426 1.529-2.33 2.779-1.643l11.54 6.348c1.295.712 1.295 2.573 0 3.285L7.28 19.991c-1.25.687-2.779-.217-2.779-1.643V5.653z" clip-rule="evenodd" />
                        </svg>
                    </div>
                </div>
            </div>

            <!-- Phone Overlay -->
            <div class="absolute bottom-0 right-10 w-48 md:w-64 transform translate-y-1/4">
                 <div class="relative mx-auto border-gray-800 bg-gray-800 border-[8px] rounded-[2rem] h-[300px] w-full shadow-xl">
                    <div class="rounded-[1.5rem] overflow-hidden w-full h-full bg-white relative flex flex-col">
                        <!-- Video/Content Area -->
                        <div class="h-2/3 relative">
                            <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" alt="Profile" class="w-full h-full object-cover" />
                            <div class="absolute inset-0 bg-black/20"></div>
                            <div class="absolute top-4 left-4 right-4 flex justify-between items-center text-white">
                                <div class="w-8 h-1 bg-white/50 rounded-full overflow-hidden">
                                    <div class="w-full h-full bg-white"></div>
                                </div>
                                <div class="w-8 h-1 bg-white/50 rounded-full"></div>
                                <div class="w-8 h-1 bg-white/50 rounded-full"></div>
                                <div class="w-6 h-6 rounded-full bg-white/20 flex items-center justify-center text-xs">✕</div>
                            </div>
                        </div>
                        
                        <!-- Bottom Sheet / Completion -->
                        <div class="absolute bottom-0 left-0 right-0 bg-white rounded-t-2xl p-4 shadow-[0_-4px_20px_rgba(0,0,0,0.1)]">
                            <div class="w-10 h-1 bg-gray-200 rounded-full mx-auto mb-4"></div>
                            <div class="flex items-center gap-3 mb-3">
                                <div class="w-8 h-8 rounded-full bg-green-100 flex items-center justify-center text-green-600">
                                    <svg class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-sm text-gray-900">Training Complete!</h4>
                                    <p class="text-[10px] text-gray-500">You scored 100% on the quiz.</p>
                                </div>
                            </div>
                            <button class="w-full bg-blue-600 text-white text-xs font-bold py-2.5 rounded-lg">Continue</button>
                        </div>
                    </div>
                 </div>
            </div>
            
            <div class="absolute top-6 left-6 bg-black/50 text-white px-3 py-1 rounded text-sm font-medium flex items-center gap-2">
                <span>▶ 10:00</span>
            </div>
        </div>

        <!-- Navigation Tabs -->
        <div class="flex flex-wrap justify-center gap-2 md:gap-4 mt-8">
            {#each ['Training', 'Checklists', 'Dashboard', 'Communication', 'Audits', 'AI Search'] as item, i}
                <button class="px-6 py-3 rounded-xl text-sm font-medium transition-all duration-300 border border-transparent hover:border-gray-200 hover:bg-gray-50 flex flex-col items-center gap-1 group {i === 0 ? 'bg-gray-900 text-white hover:bg-gray-800 hover:border-transparent' : 'text-gray-500 bg-white shadow-sm border-gray-100'}">
                    <span>{item}</span>
                    <span class="text-[10px] opacity-60 font-normal">{i === 0 ? 'Build skills fast' : 'Run work right'}</span>
                </button>
            {/each}
        </div>
    </div>
</section>
