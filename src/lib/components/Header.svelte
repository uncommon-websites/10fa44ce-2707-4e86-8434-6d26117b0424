<script lang="ts">
    import { page } from '$app/stores';
</script>

<header class="fixed w-full top-0 z-50 bg-white/80 backdrop-blur-md border-b border-gray-100 transition-all duration-300">
    <div class="container mx-auto px-4 max-w-7xl h-20 flex items-center justify-between">
        <!-- Logo -->
        <a href="/" class="flex items-center gap-2">
            <div class="w-8 h-8 text-gray-900">
                <svg viewBox="0 0 111 132" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M55.363 13.7842V65.7772L43.5135 59.006C22.4745 46.9146 9.41574 24.4246 9.41574 0H0.709961V59.4896C0.709961 78.8359 11.834 96.7311 29.4875 105.195L55.6049 117.77V65.7772L67.4544 72.5483C88.4934 84.6397 101.552 107.13 101.552 131.554H110.258V72.0646C110.258 52.7184 99.1339 34.8232 81.4804 26.3592L55.363 13.7842Z" fill="currentColor"/>
                </svg>
            </div>
            <span class="font-bold text-xl tracking-tight">SwimFlow</span>
        </a>

        <!-- Desktop Nav -->
        <nav class="hidden lg:flex items-center gap-8 text-sm font-medium text-gray-600">
            <div class="group relative cursor-pointer py-2">
                <span class="hover:text-black transition-colors flex items-center gap-1">
                    Product
                    <svg class="w-3 h-3" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" /></svg>
                </span>
            </div>
            <div class="group relative cursor-pointer py-2">
                <span class="hover:text-black transition-colors flex items-center gap-1">
                    Features
                    <svg class="w-3 h-3" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" /></svg>
                </span>
            </div>
            <a href="#" class="hover:text-black transition-colors">Pricing</a>
            <a href="#" class="hover:text-black transition-colors">About</a>
        </nav>

        <!-- Right Actions -->
        <div class="flex items-center gap-4">
            <a href="#" class="text-sm font-medium text-gray-900 hover:text-gray-600 hidden md:block">Sign in</a>
            <button class="bg-black text-white px-5 py-2.5 rounded-full text-sm font-bold hover:bg-gray-800 transition-colors">
                Book a demo
            </button>
            
            <!-- Mobile Menu Button -->
            <button class="lg:hidden p-2 text-gray-600">
                <svg class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                </svg>
            </button>
        </div>
    </div>
</header>
