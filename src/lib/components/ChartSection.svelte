<section class="py-20 border-b border-border">
	<div class="container-custom">
		<div class="flex flex-col md:flex-row justify-between items-start mb-16 gap-8">
			<div>
				<h2 class="text-3xl font-medium mb-2">Unprecedented speed with quantum accuracy</h2>
				<p class="text-xl text-muted font-light">Performance comparison across quantum chemistry methods</p>
			</div>
			<div class="max-w-xs text-[10px] text-muted leading-relaxed border-l border-border pl-4">
				<strong class="text-foreground block mb-1">About this benchmark</strong>
				Performance measured on binding free energy predictions for covalent binders. QDX EXESS achieves 1000× speed advantage over traditional ab initio methods while maintaining full quantum mechanical accuracy. Binding predictions completed in 0.3 GPU hours vs. 200-800 GPU hours for classical FEP methods. Learn more in our <a href="#" class="underline">Gordon Bell Prize publication</a>.
			</div>
		</div>

		<div class="relative w-full h-[500px] border border-border bg-primary-50/30 p-8 font-mono text-xs">
			<!-- Chart Grid -->
			<div class="absolute inset-0 p-8 grid grid-rows-6 grid-cols-1">
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
				<div class="border-b border-dashed border-gray-200 w-full h-full"></div>
			</div>
			
			<!-- Y Axis Label -->
			<div class="absolute left-2 top-1/2 -translate-y-1/2 -rotate-90 text-muted origin-center whitespace-nowrap">
				QUANTUM ACCURACY (%)
			</div>

			<!-- X Axis Label -->
			<div class="absolute bottom-2 left-1/2 -translate-x-1/2 text-muted">
				COMPUTE TIME (GPU HOURS)
			</div>

			<!-- Top Left Legend -->
			<div class="absolute top-4 left-4 flex gap-4 text-[10px] text-muted">
				<span class="bg-gray-200 px-1 rounded text-foreground">Binding Free Energy</span>
				<span>Covalent Binders</span>
				<span>Ab Initio MD</span>
			</div>

			<!-- Data Points -->
			
			<!-- QDX EXESS (The Winner) -->
			<div class="absolute top-[12%] left-[8%] flex flex-col items-center group cursor-pointer z-10">
				<div class="flex items-center gap-2 mb-1">
					<span class="text-accent font-bold">QDX EXESS</span>
				</div>
				<div class="w-3 h-3 bg-accent rounded-full shadow-[0_0_0_4px_rgba(255,68,0,0.2)]"></div>
				<div class="mt-1 text-[10px] text-accent">100% QM / 0.3h</div>
			</div>

			<!-- Traditional Ab Initio -->
			<div class="absolute top-[15%] right-[15%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-0 group-hover:opacity-100 transition-opacity">
					<span class="font-bold text-[10px]">TRADITIONAL AB INITIO</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">100% QM / 300h</div>
			</div>

			<!-- Schrödinger FEP -->
			<div class="absolute top-[70%] left-[35%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-100">
					<span class="font-bold text-[10px]">SCHRÖDINGER FEP</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">0% QM / 400h</div>
			</div>

			<!-- Gaussian -->
			<div class="absolute top-[25%] right-[25%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-100">
					<span class="font-bold text-[10px]">GAUSSIAN</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">100% QM / 500h</div>
			</div>

			<!-- Classical MD -->
			<div class="absolute top-[75%] left-[25%] flex flex-col items-center group cursor-pointer">
				<div class="flex items-center gap-2 mb-1 opacity-100">
					<span class="font-bold text-[10px]">CLASSICAL MD</span>
				</div>
				<div class="w-2 h-2 bg-black rounded-full"></div>
				<div class="mt-1 text-[10px] text-muted">0% QM / 200h</div>
			</div>

			<!-- Bottom Right Legend -->
			<div class="absolute bottom-4 right-4 flex items-center gap-4 text-[10px]">
				<div class="flex items-center gap-1">
					<div class="w-2 h-2 bg-accent rounded-full"></div>
					<span class="text-accent font-bold">QDX EXESS</span>
				</div>
				<div class="flex items-center gap-1">
					<div class="w-2 h-2 bg-black rounded-full"></div>
					<span class="text-muted">COMPETITORS</span>
				</div>
			</div>
		</div>
	</div>
</section>
