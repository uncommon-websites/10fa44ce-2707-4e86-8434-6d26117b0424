<script lang="ts">
    let selectedRange = '1 - 5';
    const ranges = ['1 - 5', '6 - 10', '11 - 20', '21 - 50', '51 - 100', '100+'];
    
    // Simple logic to change values based on selection
    $: multiplier = ranges.indexOf(selectedRange) + 1;
    $: adminSavings = (15 * multiplier).toFixed(0);
    $: revenueRecovery = (2 * multiplier).toFixed(1);
    $: growthPotential = (25 * multiplier).toFixed(0);
</script>

<section class="py-20 bg-gray-50/50">
    <div class="container mx-auto px-4 max-w-4xl">
        <div class="text-center mb-12">
            <span class="text-primary-600 font-semibold tracking-wider text-xs uppercase mb-4 block">ROI Calculator</span>
            <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
                Calculate your potential<br />
                savings with SwimFlow
            </h2>
        </div>

        <div class="bg-white rounded-3xl shadow-xl p-8 md:p-12">
            <div class="mb-12">
                <label class="block text-sm font-bold text-gray-900 mb-4">How many locations do you operate?</label>
                <div class="grid grid-cols-2 md:grid-cols-3 gap-3">
                    {#each ranges as range}
                        <button 
                            class="px-4 py-3 rounded-xl text-sm font-medium transition-all duration-200 border 
                            {selectedRange === range 
                                ? 'bg-primary-50 border-primary-200 text-primary-600 ring-1 ring-primary-200' 
                                : 'bg-white border-gray-200 text-gray-600 hover:border-gray-300'}"
                            on:click={() => selectedRange = range}
                        >
                            {range}
                        </button>
                    {/each}
                </div>
            </div>

            <div class="border-t border-gray-100 pt-12 text-center">
                <div class="text-xs font-bold text-gray-400 uppercase tracking-widest mb-6">Estimated Impact</div>
                <h3 class="text-2xl font-bold text-gray-900 mb-8">Your potential ROI with SwimFlow</h3>
                <p class="text-gray-500 text-sm mb-8 max-w-lg mx-auto">
                    Based on data from operators who switched from manual tools to our unified platform.
                </p>

                <div class="space-y-4 max-w-lg mx-auto mb-12">
                    <div class="flex justify-between items-center py-3 border-b border-gray-50">
                        <div class="flex items-center gap-2 text-sm text-gray-600 text-left">
                            Admin hours saved weekly
                        </div>
                        <div class="font-bold text-primary-600 bg-primary-50 px-3 py-1 rounded-lg">{adminSavings} hrs</div>
                    </div>
                    <div class="flex justify-between items-center py-3 border-b border-gray-50">
                        <div class="flex items-center gap-2 text-sm text-gray-600 text-left">
                            Revenue recovered monthly (failed payments)
                        </div>
                        <div class="font-bold text-primary-600 bg-primary-50 px-3 py-1 rounded-lg">${revenueRecovery}K</div>
                    </div>
                </div>

                <div class="mb-2 text-sm font-bold text-gray-900">Annual Growth Potential</div>
                <div class="text-6xl md:text-7xl font-bold text-primary-600">${growthPotential}K</div>
            </div>
        </div>
    </div>
</section>