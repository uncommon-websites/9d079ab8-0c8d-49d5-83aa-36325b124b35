<script lang="ts">
	import FeatureBlock from './FeatureBlock.svelte';
</script>

<!-- Block 1: EXESS Platform -->
<FeatureBlock 
	title="EXESS: Ultra-fast quantum chemistry" 
	description="Our flagship platform runs 1000× faster than state-of-the-art, compressing a year of compute into hours."
	buttons={[
		{ text: "REQUEST ACCESS", icon: true },
		{ text: "VIEW BENCHMARKS" }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 font-mono text-xs">
		<div class="flex items-center gap-2 border-b border-border pb-2 mb-4">
			<span class="text-accent">></span>
			<span class="text-muted">EXESS Simulation</span>
			<span class="w-2 h-4 bg-accent animate-pulse"></span>
		</div>
		<div class="space-y-3">
			<div class="flex justify-between items-center">
				<span class="text-muted text-[10px]">System size:</span>
				<span class="text-foreground">1,048,576 electrons</span>
			</div>
			<div class="flex justify-between items-center">
				<span class="text-muted text-[10px]">Performance:</span>
				<span class="text-accent">1.1 EFLOP/s</span>
			</div>
			<div class="flex justify-between items-center">
				<span class="text-muted text-[10px]">Method:</span>
				<span class="text-foreground">Ab initio MD</span>
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 2: Covalent Binder Simulations -->
<FeatureBlock 
	title="Covalent binder design and prediction" 
	description="Simulate irreversible covalent binders with bond breaking and formation that classical methods cannot model"
	buttons={[
		{ text: "EXPLORE CAPABILITIES", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full max-w-md bg-white border border-border rounded shadow-sm p-6 flex flex-col gap-4">
		<div class="flex items-center gap-2 text-xs font-mono text-muted">
			<div class="w-4 h-4 border border-current rounded-sm flex items-center justify-center">
				<div class="w-2 h-2 bg-current rounded-[1px]"></div>
			</div>
			Simulating covalent binding...
		</div>
		<div class="w-full bg-gray-100 h-1.5 rounded-full overflow-hidden">
			<div class="bg-accent h-full w-2/3"></div>
		</div>
		<div class="space-y-2 text-[10px] font-mono">
			<div class="flex items-center gap-2">
				<span class="w-2 h-2 bg-green-500 rounded-full"></span>
				<span class="text-muted">Cysteine binding complete</span>
			</div>
			<div class="flex items-center gap-2">
				<span class="w-2 h-2 bg-green-500 rounded-full"></span>
				<span class="text-muted">Lysine binding complete</span>
			</div>
			<div class="flex items-center gap-2">
				<span class="w-2 h-2 bg-accent rounded-full animate-pulse"></span>
				<span class="text-foreground">Serine binding in progress</span>
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 3: CYP450 Metabolism Prediction -->
<FeatureBlock 
	title="CYP450 metabolism simulation" 
	description="Address the $12B annual industry cost from CYP liabilities with quantum-accurate enzyme metabolism predictions"
	buttons={[
		{ text: "LEARN MORE", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>ENZYME</div>
			<div>SUBSTRATE</div>
			<div>PREDICTION</div>
			<div>CONFIDENCE</div>
		</div>
		{#each [
			{ enzyme: 'CYP3A4', substrate: 'Compound A', pred: 'Metabolized', conf: 95 },
			{ enzyme: 'CYP2D6', substrate: 'Compound B', pred: 'Stable', conf: 92 },
			{ enzyme: 'CYP2C9', substrate: 'Compound C', pred: 'Metabolized', conf: 88 },
			{ enzyme: 'CYP1A2', substrate: 'Compound D', pred: 'Stable', conf: 91 },
			{ enzyme: 'CYP2C19', substrate: 'Compound E', pred: 'Metabolized', conf: 94 },
			{ enzyme: 'CYP2E1', substrate: 'Compound F', pred: 'Stable', conf: 89 }
		] as row}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="text-primary-600 font-semibold">{row.enzyme}</div>
				<div class="text-muted">{row.substrate}</div>
				<div class="text-foreground">{row.pred}</div>
				<div class="flex items-center gap-1">
					<div class="h-1.5 w-8 bg-gray-100 rounded overflow-hidden">
						<div class="h-full bg-accent" style="width: {row.conf}%"></div>
					</div>
					<span class="text-muted">{row.conf}%</span>
				</div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 4: Hamiltonian-Preserving ML -->
<FeatureBlock 
	title="Hamiltonian-preserving neural networks" 
	description="NN-xTB models achieve DFT-level accuracy at xTB speed with adaptive quantum replicas for ground-truth validation"
	buttons={[
		{ text: "VIEW RESEARCH", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-3 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>METHOD</div>
			<div>ACCURACY</div>
			<div>SPEED</div>
		</div>
		{#each [
			{ method: 'NN-xTB', accuracy: 'DFT-level', speed: 'xTB speed', highlight: true },
			{ method: 'Traditional DFT', accuracy: 'High', speed: 'Slow', highlight: false },
			{ method: 'Classical xTB', accuracy: 'Medium', speed: 'Fast', highlight: false },
			{ method: 'Force Fields', accuracy: 'Low', speed: 'Very Fast', highlight: false },
			{ method: 'AQR (Adaptive)', accuracy: 'DFT-level', speed: 'Fast', highlight: true },
			{ method: 'Pure ML', accuracy: 'Variable', speed: 'Fast', highlight: false }
		] as row}
			<div class="grid grid-cols-3 gap-2 p-2 border-b border-border/50 items-center {row.highlight ? 'bg-primary-50/50' : ''}">
				<div class="font-semibold {row.highlight ? 'text-primary-600' : 'text-foreground'}">{row.method}</div>
				<div class="text-muted">{row.accuracy}</div>
				<div class="text-muted">{row.speed}</div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 5: Exascale Infrastructure -->
<FeatureBlock 
	title="Massively parallel exascale infrastructure" 
	description="First team to break the million-electron and 1 EFLOP/s barriers in biomolecular-scale ab initio molecular dynamics"
	buttons={[
		{ text: "VIEW ARCHITECTURE", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 flex flex-col gap-4">
		<div class="flex items-center justify-between border-b border-border pb-2">
			<div class="text-[10px] font-mono text-muted flex items-center gap-2">
				<span class="w-2 h-2 bg-green-500 rounded-full"></span>
				Exascale compute cluster active
			</div>
		</div>
		
		<!-- Performance Grid visual -->
		<div class="grid grid-cols-12 gap-1">
			{#each Array(48) as _, i}
				<div class="aspect-square rounded-[1px] {i < 42 ? 'bg-accent' : (i < 45 ? 'bg-primary-300' : 'bg-gray-100')}"></div>
			{/each}
		</div>

		<div class="mt-auto space-y-3">
			<div class="flex justify-between items-center text-[10px] font-mono">
				<span class="text-muted">Current throughput:</span>
				<span class="text-accent font-bold">1.1 EFLOP/s</span>
			</div>
			<div class="flex justify-between items-center text-[10px] font-mono">
				<span class="text-muted">World records held:</span>
				<span class="text-foreground font-bold">4</span>
			</div>
			<div class="bg-gray-50 p-2 rounded border border-border text-[10px] font-mono text-center text-muted">
				Gordon Bell Prize 2024
			</div>
		</div>
	</div>
</FeatureBlock>
