<section class="py-20 border-b border-border">
	<div class="container-custom">
		<div class="grid grid-cols-1 md:grid-cols-2 gap-16">
			
			<!-- Left Column: CTA & Visual -->
			<div class="flex flex-col h-full">
				<div class="mb-8">
					<p class="font-mono text-xs text-muted mb-4">Partner with us</p>
					<h2 class="text-2xl font-medium mb-4">Transforming drug discovery through quantum simulations</h2>
					<p class="text-muted font-light mb-8 text-sm leading-relaxed max-w-md">
						QDX is pioneering ultra-fast ab initio quantum chemistry to simulate nature's most complex systems
					</p>
					<div class="flex gap-3 mb-12">
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							REQUEST DEMO
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">D</span>
						</button>
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							VIEW RESEARCH
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">R</span>
						</button>
					</div>
				</div>
				
				<!-- Molecular Visual -->
				<div class="mt-auto w-full h-48 bg-black relative overflow-hidden flex items-center justify-center">
					{#each Array(100) as _, i}
						<div 
							class="h-full bg-white absolute" 
							style="
								left: {i}%; 
								width: {Math.random() * 2}%; 
								opacity: {Math.random()};
							"
						></div>
					{/each}
					<div class="absolute inset-0 flex items-center justify-center">
						<div class="bg-black text-white font-mono text-[10px] px-2 py-1 z-10">
							QDX.EXASCALE
						</div>
					</div>
				</div>
			</div>

			<!-- Right Column: Updates -->
			<div>
				<p class="font-mono text-xs text-muted mb-8">Latest milestones</p>
				
				<div class="space-y-12">
					<!-- Update 1 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">January 2025</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Prof. Giuseppe Barca awarded 2025 WATOC Dirac Medal</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								QDX Chief Scientist Giuseppe Barca receives the prestigious Dirac Medal for outstanding contributions to theoretical and computational chemistry. The award recognizes his pioneering work in biomolecular-scale quantum simulations and breakthrough achievements in exascale computing.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Award</span>
						</div>
					</div>

					<!-- Update 2 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">November 2024</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">QDX team wins 2024 ACM Gordon Bell Prize</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								The "Nobel Prize of High Performance Computing" awarded to QDX for pioneering quantum-accurate simulations of biomolecular systems at exascale. First team to break the million-electron and 1 EFLOP/s barriers in ab initio molecular dynamics, achieving 1000× speed improvements over previous state-of-the-art.
							</p>
							<div class="flex gap-2">
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Award</span>
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Research</span>
							</div>
						</div>
					</div>

					<!-- Update 3 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">October 2024</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Prelude Therapeutics partnership delivers breakthrough in JAK2 selectivity</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								QDX collaboration with Prelude Therapeutics on JAK2 V617F mutation resulted in discovery of previously unknown deep pocket and compound with unprecedented selectivity. Prelude optioned their mutant selective JAK2V617F JH2 inhibitor program in deal worth nearly $1 billion.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Partnership</span>
						</div>
					</div>

					<!-- Update 4 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">2024</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">QDX sets four world records in quantum chemistry simulations</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								QDX holds world records for fastest and largest ab initio quantum chemistry simulations, demonstrating unprecedented capabilities in biomolecular-scale quantum mechanical calculations.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Achievement</span>
						</div>
					</div>
				</div>
			</div>

		</div>
	</div>
</section>
