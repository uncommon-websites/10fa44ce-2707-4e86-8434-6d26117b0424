<section class="py-20 bg-white">
    <div class="container mx-auto px-4 max-w-7xl">
        <div class="text-center mb-12">
            <span class="text-primary-600 font-semibold tracking-wider text-xs uppercase mb-4 block">Testimonials</span>
            <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">
                Why operators love SwimFlow
            </h2>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <!-- Testimonial 1 -->
            <div class="group cursor-pointer">
                <div class="relative rounded-2xl overflow-hidden aspect-[4/3] mb-4">
                    <img src="/generated/image-a-happy-parent-looking-at-their-phone-an-1768533804061-3.webp" alt="Sarah Jenkins" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />
                    <div class="absolute inset-0 bg-black/20 flex items-center justify-center">
                        <div class="w-12 h-12 bg-white/30 backdrop-blur rounded-full flex items-center justify-center group-hover:bg-white transition-colors">
                            <svg class="w-5 h-5 text-white group-hover:text-black ml-1" fill="currentColor" viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg>
                        </div>
                    </div>
                </div>
                <h4 class="font-bold text-gray-900">Sarah Jenkins</h4>
                <p class="text-gray-500 text-sm">Blue Wave Swim School</p>
            </div>

            <!-- Testimonial 2 -->
            <div class="group cursor-pointer">
                <div class="relative rounded-2xl overflow-hidden aspect-[4/3] mb-4">
                    <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Mark Thompson" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />
                    <div class="absolute inset-0 bg-black/20 flex items-center justify-center">
                        <div class="w-12 h-12 bg-white/30 backdrop-blur rounded-full flex items-center justify-center group-hover:bg-white transition-colors">
                            <svg class="w-5 h-5 text-white group-hover:text-black ml-1" fill="currentColor" viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg>
                        </div>
                    </div>
                </div>
                <h4 class="font-bold text-gray-900">Mark Thompson</h4>
                <p class="text-gray-500 text-sm">AquaKids Academy</p>
            </div>

            <!-- Testimonial 3 -->
            <div class="group">
                <div class="bg-primary-50 rounded-2xl p-8 h-full flex flex-col justify-center">
                    <div class="text-primary-600 mb-4">
                        {#each Array(5) as _}
                            <span class="text-xl">★</span>
                        {/each}
                    </div>
                    <p class="text-gray-700 italic mb-6">"SwimFlow has completely transformed how we handle our waitlists and billing. We've saved at least 15 hours of admin work every single week."</p>
                    <div>
                        <div class="font-bold text-gray-900">Jessica Miller</div>
                        <div class="text-sm text-gray-500">Director, Splash Sports</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
