<script lang="ts">
    let selectedRange = '11 - 50';
    const ranges = ['11 - 50', '51 - 100', '101 - 500', '501 - 1000', '1001 - 5000', '5001+'];
    
    // Simple logic to change values based on selection
    $: multiplier = ranges.indexOf(selectedRange) + 1;
    $: onboardingSavings = (3.6 * multiplier).toFixed(1);
    $: turnoverSavings = (4.5 * multiplier).toFixed(1);
    $: revenueIncrease = (30 * multiplier).toFixed(0);
</script>

<section class="py-20 bg-gray-50/50">
    <div class="container mx-auto px-4 max-w-4xl">
        <div class="text-center mb-12">
            <span class="text-blue-500 font-semibold tracking-wider text-xs uppercase mb-4 block">ROI Calculator</span>
            <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
                Calculate your potential<br />
                ROI with Bounti
            </h2>
        </div>

        <div class="bg-white rounded-3xl shadow-xl p-8 md:p-12">
            <div class="mb-12">
                <label class="block text-sm font-bold text-gray-900 mb-4">How many employees do you have?</label>
                <div class="grid grid-cols-2 md:grid-cols-3 gap-3">
                    {#each ranges as range}
                        <button 
                            class="px-4 py-3 rounded-xl text-sm font-medium transition-all duration-200 border 
                            {selectedRange === range 
                                ? 'bg-blue-50 border-blue-200 text-blue-600 ring-1 ring-blue-200' 
                                : 'bg-white border-gray-200 text-gray-600 hover:border-gray-300'}"
                            on:click={() => selectedRange = range}
                        >
                            {range}
                        </button>
                    {/each}
                </div>
            </div>

            <div class="border-t border-gray-100 pt-12 text-center">
                <div class="text-xs font-bold text-gray-400 uppercase tracking-widest mb-6">Estimated ROI</div>
                <h3 class="text-2xl font-bold text-gray-900 mb-8">Your potential ROI with Bounti</h3>
                <p class="text-gray-500 text-sm mb-8 max-w-lg mx-auto">
                    Bounti has been developed in Germany. We aim to bring transparency to your operations.
                </p>

                <div class="space-y-4 max-w-lg mx-auto mb-12">
                    <div class="flex justify-between items-center py-3 border-b border-gray-50">
                        <div class="flex items-center gap-2 text-sm text-gray-600">
                            <span class="text-blue-500 font-bold">€</span> Savings in onboarding costs yearly
                        </div>
                        <div class="font-bold text-blue-500 bg-blue-50 px-3 py-1 rounded-lg">€{onboardingSavings}K</div>
                    </div>
                    <div class="flex justify-between items-center py-3 border-b border-gray-50">
                        <div class="flex items-center gap-2 text-sm text-gray-600">
                            <span class="text-blue-500 font-bold">€</span> Savings in turnover costs yearly
                        </div>
                        <div class="font-bold text-blue-500 bg-blue-50 px-3 py-1 rounded-lg">€{turnoverSavings}K</div>
                    </div>
                </div>

                <div class="mb-2 text-sm font-bold text-gray-900">Revenue increase through Productivity Gains</div>
                <div class="text-6xl md:text-7xl font-bold text-green-500">€{revenueIncrease}K</div>
            </div>
        </div>
    </div>
</section>