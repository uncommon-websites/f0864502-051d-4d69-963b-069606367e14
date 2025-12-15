<section class="py-24 bg-white border-t border-gray-200 font-sans">
    <div class="max-w-7xl mx-auto px-4 text-center mb-16">
        <span class="text-[10px] font-bold text-gray-500 uppercase tracking-widest border border-gray-200 px-3 py-1.5 rounded-full bg-gray-50">Clinical Training & Support</span>
        <h2 class="mt-8 text-5xl md:text-6xl font-serif-display text-gray-900">Get your team up to speed <br/> in minutes, not months</h2>
        <p class="mt-6 text-gray-600 max-w-2xl mx-auto">Comprehensive training and ongoing support ensure your clinical team can leverage Cleo's full capabilities from day one.</p>
        <div class="mt-8">
            <a href="#" class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-sm font-bold rounded bg-gray-900 text-white hover:bg-gray-800 transition-colors">
                View Training Resources ->
            </a>
        </div>
    </div>

    <!-- Video Grid (Mockup) -->
    <div class="max-w-7xl mx-auto px-4">
        <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
            {#each Array(8) as _, i}
            <div class="aspect-video bg-gray-200 rounded-lg overflow-hidden relative group cursor-pointer">
                <img src={`https://placehold.co/400x225/333/fff?text=Video+${i+1}`} alt="Video Thumbnail" class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-300" />
                <div class="absolute inset-0 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity bg-black/20">
                    <div class="w-10 h-10 bg-white rounded-full flex items-center justify-center">
                        <svg class="w-4 h-4 ml-0.5" fill="currentColor" viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg>
                    </div>
                </div>
            </div>
            {/each}
        </div>
        
        <!-- Quote -->
        <div class="mt-12 flex flex-col md:flex-row items-center gap-8 max-w-5xl mx-auto">
            <div class="w-24 h-24 md:w-32 md:h-32 rounded-full overflow-hidden flex-shrink-0 border-2 border-gray-100">
                <img src="https://placehold.co/200x200/eee/333?text=User" alt="User" class="w-full h-full object-cover" />
            </div>
            <div class="flex-1 text-center md:text-left">
                <blockquote class="text-2xl md:text-3xl font-serif-display text-gray-700 leading-tight">
                    "The onboarding was seamless. Our entire ED team was comfortable using Cleo within the first week."
                </blockquote>
                <div class="mt-4 text-xs font-bold uppercase tracking-widest text-gray-400">
                    Dr. Michael Chen <br/>
                    <span class="text-gray-300">Chief Medical Officer, Trinity Health</span>
                </div>
            </div>
        </div>
    </div>
</section>
