<script>
    // No script logic needed for this static recreation yet
</script>

<section class="py-20 bg-white font-sans">
    <div class="max-w-7xl mx-auto px-4 text-center">
        <span class="text-[10px] font-bold text-gray-500 uppercase tracking-widest border border-gray-200 px-3 py-1.5 rounded-full bg-gray-50">The Cleo Platform</span>
        <h2 class="mt-8 text-5xl md:text-7xl font-serif-display text-gray-900 leading-tight">Complete acute care <br/> coverage from <br/> entry to followup</h2>
    </div>
    
    <!-- Tabbed interface image area -->
    <div class="max-w-7xl mx-auto mt-16 px-4">
        <div class="border border-gray-200 rounded-xl overflow-hidden shadow-sm bg-white grid md:grid-cols-12 min-h-[600px]">
             <div class="md:col-span-4 p-8 md:p-12 border-r border-gray-200 flex flex-col justify-center">
                 <h3 class="text-3xl font-serif-display mb-4">Real-time ambient documentation</h3>
                 <p class="text-gray-600 text-base leading-relaxed mb-8">Cleo captures clinical encounters in real-time, transforming chaotic ED workflows into structured, accurate notes. Our AI understands medical terminology, clinical context, and documentation requirements—so you don't have to think about it.</p>
                 <div>
                    <button class="text-sm font-bold border-b border-gray-300 pb-0.5 hover:border-gray-900 transition-colors">Learn More -></button>
                 </div>
             </div>
             <div class="md:col-span-8 bg-gray-50 p-8 md:p-12 flex items-center justify-center relative overflow-hidden">
                 <!-- Simplified UI Mockup -->
                 <div class="bg-white shadow-xl rounded-lg w-full h-full border border-gray-200 p-6 relative flex flex-col">
                    <div class="flex gap-2 mb-6 border-b border-gray-100 pb-4">
                        <div class="w-3 h-3 rounded-full bg-red-400"></div>
                        <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
                        <div class="w-3 h-3 rounded-full bg-green-400"></div>
                        <div class="ml-auto flex gap-2">
                            <div class="h-4 w-32 bg-gray-100 rounded-full"></div>
                        </div>
                    </div>
                    
                    <div class="space-y-6">
                        <!-- Header Stats -->
                        <div class="grid grid-cols-4 gap-4">
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Patients</div>
                                 <div class="text-xl font-bold text-gray-900">342</div>
                                 <div class="text-[10px] text-blue-600 font-bold">Today</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Avg Time</div>
                                 <div class="text-xl font-bold text-gray-900">4.2m</div>
                                 <div class="text-[10px] text-green-600 font-bold">-60%</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Accuracy</div>
                                 <div class="text-xl font-bold text-gray-900">98.7%</div>
                                 <div class="text-[10px] text-green-600 font-bold">+2.1%</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Charges</div>
                                 <div class="text-xl font-bold text-gray-900">$847k</div>
                                 <div class="text-[10px] text-gray-400 font-bold">MTD</div>
                             </div>
                        </div>

                        <!-- Data Table -->
                        <div class="border border-gray-100 rounded-lg overflow-hidden">
                            <div class="bg-gray-50 px-4 py-2 border-b border-gray-100 flex text-[10px] font-bold text-gray-500 uppercase tracking-wider">
                                <div class="w-1/3">Patient</div>
                                <div class="w-1/6 text-right">Time</div>
                                <div class="w-1/6 text-right">Status</div>
                                <div class="w-1/6 text-right">Provider</div>
                                <div class="w-1/6 text-right">Action</div>
                            </div>
                            <div class="divide-y divide-gray-50 text-xs">
                                 {#each [
                                     {patient: 'Smith, J. - 45F', time: '2m', status: 'Complete', provider: 'Dr. Chen', action: 'Reviewed'},
                                     {patient: 'Johnson, M. - 62M', time: '5m', status: 'In Progress', provider: 'Dr. Patel', action: 'Active'},
                                     {patient: 'Williams, S. - 28F', time: '3m', status: 'Complete', provider: 'Dr. Lee', action: 'Signed'},
                                     {patient: 'Brown, R. - 71M', time: '7m', status: 'Review', provider: 'Dr. Garcia', action: 'Pending'},
                                     {patient: 'Davis, K. - 34F', time: '4m', status: 'Complete', provider: 'Dr. Chen', action: 'Reviewed'}
                                 ] as item}
                                 <div class="px-4 py-3 flex items-center hover:bg-gray-50 transition-colors">
                                     <div class="w-1/3 font-medium text-gray-900">{item.patient}</div>
                                     <div class="w-1/6 text-right text-gray-600">{item.time}</div>
                                     <div class="w-1/6 text-right">
                                         <span class="px-1.5 py-0.5 rounded text-[10px] font-bold {item.status === 'Complete' ? 'bg-green-100 text-green-700' : item.status === 'In Progress' ? 'bg-blue-100 text-blue-700' : 'bg-yellow-100 text-yellow-700'}">{item.status}</span>
                                     </div>
                                     <div class="w-1/6 text-right text-gray-600">{item.provider}</div>
                                     <div class="w-1/6 text-right">
                                         <span class="text-[10px] font-bold text-gray-900">{item.action}</span>
                                     </div>
                                 </div>
                                 {/each}
                            </div>
                        </div>
                    </div>
                 </div>
             </div>
        </div>
        
        <!-- Bottom Grid of 3 items -->
        <div class="grid md:grid-cols-3 gap-0 mt-0 border-x border-b border-gray-200 divide-x divide-gray-200 bg-white">
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">1</div>
                <p class="text-xs text-gray-600 leading-relaxed">Capture clinical encounters in real-time with ambient AI that understands medical context and documentation requirements.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">2</div>
                <p class="text-xs text-gray-600 leading-relaxed">Seamlessly integrate with Epic, Cerner, and Athena to ensure documentation flows directly into your existing EHR.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">3</div>
                <p class="text-xs text-gray-600 leading-relaxed">Reduce documentation time by 60% while improving accuracy and charge capture—giving clinicians time back for patient care.</p>
            </div>
        </div>
    </div>
</section>