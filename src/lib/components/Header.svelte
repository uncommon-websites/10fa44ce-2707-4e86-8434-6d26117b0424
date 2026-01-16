<script lang="ts">
    import { page } from '$app/stores';
</script>

<header class="fixed w-full top-0 z-50 bg-white/80 backdrop-blur-md border-b border-gray-100 transition-all duration-300">
    <div class="container mx-auto px-4 max-w-7xl h-20 flex items-center justify-between">
        <!-- Logo -->
        <a href="/" class="flex items-center gap-2">
            <div class="w-8 h-8 text-primary-600">
                <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M22.0368 13.2272C22.0369 13.8625 21.9118 14.4916 21.6687 15.0785C21.4255 15.6654 21.0691 16.1986 20.6197 16.6476C20.1703 17.0967 19.6368 17.4527 19.0497 17.6953C18.4624 17.938 17.8333 18.0625 17.1979 18.0618H15.9157L15.7023 15.1819C15.6638 14.079 15.3908 12.9969 14.9014 12.0077C14.6066 11.4124 14.1527 10.9103 13.5899 10.5574C13.0271 10.2045 12.3775 10.0144 11.7132 10.0083C11.2203 10.007 10.7376 10.1492 10.3241 10.4175C9.9106 10.6858 9.58412 11.0687 9.3845 11.5194C8.93081 11.6396 8.51813 11.8804 8.19019 12.2162C7.86226 12.552 7.63132 12.9703 7.52183 13.4267C7.51904 13.4395 7.51991 13.4529 7.52435 13.4652C7.52879 13.4775 7.53662 13.4884 7.54694 13.4965C7.55729 13.5046 7.56977 13.5096 7.5829 13.5109C7.59601 13.5121 7.60921 13.5095 7.62089 13.5034C8.37992 13.1058 9.39707 13.1072 9.96773 13.3793C10.3975 13.5858 10.6221 14.1494 10.5607 14.649L10.237 18.0562H4.72573C4.24472 18.0656 3.76668 17.979 3.31954 17.8015C2.87241 17.624 2.46518 17.359 2.12167 17.0222C1.77816 16.6854 1.50529 16.2834 1.319 15.8399C1.13272 15.3963 1.03677 14.9201 1.03677 14.439C1.03677 13.9579 1.13272 13.4816 1.319 13.038C1.50529 12.5945 1.77816 12.1925 2.12167 11.8557C2.46518 11.5189 2.87241 11.254 3.31954 11.0764C3.76668 10.8989 4.24472 10.8123 4.72573 10.8217H5.08012C5.2504 9.50028 5.82913 8.26501 6.73547 7.28839C7.64182 6.31177 8.83054 5.64258 10.1356 5.37428C11.4407 5.10598 12.797 5.25196 14.0151 5.79183C15.2332 6.33169 16.2523 7.2385 16.9302 8.38562H17.2092C17.8441 8.38634 18.4726 8.51218 19.059 8.75593C19.6453 8.99966 20.1778 9.35654 20.626 9.80615C21.0744 10.2558 21.4297 10.7893 21.6718 11.3763C21.9139 11.9633 22.0378 12.5922 22.0368 13.2272ZM11.6393 11.2306C11.546 11.2308 11.455 11.2587 11.3776 11.3107C11.3003 11.3627 11.24 11.4365 11.2046 11.5226C11.1691 11.6088 11.1599 11.7036 11.1783 11.795C11.1966 11.8864 11.2417 11.9703 11.3077 12.0361C11.3737 12.1019 11.4577 12.1467 11.5492 12.1648C11.6406 12.1829 11.7353 12.1734 11.8214 12.1377C11.9075 12.102 11.9811 12.0415 12.0329 11.964C12.0846 11.8865 12.1123 11.7954 12.1123 11.7022C12.1123 11.6401 12.1 11.5787 12.0762 11.5214C12.0524 11.4641 12.0176 11.412 11.9736 11.3682C11.9297 11.3244 11.8775 11.2897 11.8202 11.2661C11.7628 11.2424 11.7013 11.2304 11.6393 11.2306Z" fill="currentColor"/>
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
