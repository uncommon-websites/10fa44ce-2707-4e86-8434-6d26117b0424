<section class="py-20 bg-white">
    <div class="container mx-auto px-4 max-w-6xl">
        <div class="text-center mb-12">
            <span class="text-primary-600 font-semibold tracking-wider text-xs uppercase mb-4 block">Empowering Your Team</span>
            <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">
                Boost instructor performance.<br />
                Achieve operational excellence.
            </h2>
            <p class="text-gray-600 text-lg max-w-2xl mx-auto mb-8">
                One platform that ties it all together. Manage classes, track attendance, and keep every family updated.
            </p>
            <div class="flex justify-center gap-4">
                <button class="bg-primary-600 text-white px-6 py-2.5 rounded-full font-medium hover:bg-primary-700 transition-colors">
                    Book a demo <span class="ml-1">↗</span>
                </button>
            </div>
        </div>

        <!-- Video/Image Container -->
        <div class="relative rounded-3xl overflow-hidden shadow-2xl bg-gray-900 aspect-video md:aspect-[21/9] group cursor-pointer">
            <img src="/generated/image-a-swim-school-instructor-smiling-and-int-1768533799358-1.webp" alt="Instructor teaching" class="w-full h-full object-cover opacity-80 group-hover:opacity-60 transition-opacity" />
            
            <div class="absolute inset-0 flex items-center justify-center">
                <div class="w-16 h-16 bg-white/20 backdrop-blur-sm rounded-full flex items-center justify-center group-hover:scale-110 transition-transform">
                    <div class="w-12 h-12 bg-white rounded-full flex items-center justify-center pl-1">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-6 h-6 text-primary-600">
                            <path fill-rule="evenodd" d="M4.5 5.653c0-1.426 1.529-2.33 2.779-1.643l11.54 6.348c1.295.712 1.295 2.573 0 3.285L7.28 19.991c-1.25.687-2.779-.217-2.779-1.643V5.653z" clip-rule="evenodd" />
                        </svg>
                    </div>
                </div>
            </div>

            <!-- Phone Overlay -->
            <div class="absolute bottom-0 right-10 w-48 md:w-64 transform translate-y-1/4">
                 <div class="relative mx-auto border-gray-800 bg-gray-800 border-[8px] rounded-[2rem] h-[300px] w-full shadow-xl">
                    <div class="rounded-[1.5rem] overflow-hidden w-full h-full bg-white relative flex flex-col">
                        <!-- Content Area -->
                        <div class="h-2/3 relative bg-primary-600 p-4 flex flex-col justify-center">
                            <div class="text-white font-bold text-lg mb-2">Class Check-in</div>
                            <div class="space-y-2">
                                <div class="bg-white/20 h-8 rounded flex items-center px-2">
                                    <div class="w-4 h-4 bg-green-400 rounded-full mr-2"></div>
                                    <div class="h-2 bg-white/50 rounded w-1/2"></div>
                                </div>
                                <div class="bg-white/20 h-8 rounded flex items-center px-2">
                                    <div class="w-4 h-4 bg-green-400 rounded-full mr-2"></div>
                                    <div class="h-2 bg-white/50 rounded w-2/3"></div>
                                </div>
                            </div>
                        </div>
                        
                        <!-- Bottom Sheet -->
                        <div class="absolute bottom-0 left-0 right-0 bg-white rounded-t-2xl p-4 shadow-[0_-4px_20px_rgba(0,0,0,0.1)]">
                            <div class="w-10 h-1 bg-gray-200 rounded-full mx-auto mb-4"></div>
                            <div class="flex items-center gap-3 mb-3">
                                <div class="w-8 h-8 rounded-full bg-primary-100 flex items-center justify-center text-primary-600">
                                    <svg class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" /></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-sm text-gray-900">Attendance Logged</h4>
                                    <p class="text-[10px] text-gray-500">12 students checked in.</p>
                                </div>
                            </div>
                            <button class="w-full bg-primary-600 text-white text-xs font-bold py-2.5 rounded-lg">View Schedule</button>
                        </div>
                    </div>
                 </div>
            </div>
            
            <div class="absolute top-6 left-6 bg-black/50 text-white px-3 py-1 rounded text-sm font-medium flex items-center gap-2">
                <span>▶ Watch Demo</span>
            </div>
        </div>

        <!-- Navigation Tabs -->
        <div class="flex flex-wrap justify-center gap-2 md:gap-4 mt-8">
            {#each ['Scheduling', 'Waitlists', 'Billing', 'Assessments', 'Communication', 'Reporting'] as item, i}
                <button class="px-6 py-3 rounded-xl text-sm font-medium transition-all duration-300 border border-transparent hover:border-gray-200 hover:bg-gray-50 flex flex-col items-center gap-1 group {i === 0 ? 'bg-gray-900 text-white hover:bg-gray-800 hover:border-transparent' : 'text-gray-500 bg-white shadow-sm border-gray-100'}">
                    <span>{item}</span>
                    <span class="text-[10px] opacity-60 font-normal">{i === 0 ? 'Drag-and-drop' : 'Automated flow'}</span>
                </button>
            {/each}
        </div>
    </div>
</section>
