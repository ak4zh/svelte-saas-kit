<script>
	import '@brainandbones/skeleton/themes/theme-skeleton.css';
	import '@brainandbones/skeleton/styles/all.css';
	import '../app.postcss';

	import { AppShell, AppBar, GradientHeading} from '@brainandbones/skeleton';
</script>

<AppShell>
	<svelte:fragment slot="header">
		<AppBar>
			<svelte:fragment slot="lead">
				<GradientHeading tag="h1" class="text-3xl" direction="bg-gradient-to-r" from="from-primary-500" to="to-accent-500">Skeleton</GradientHeading>
			</svelte:fragment>

			<svelte:fragment slot="trail">(trail)</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<svelte:fragment slot="sidebarLeft">
		<div id="sidebar-left" class="hidden lg:block">Sidebar</div>
	</svelte:fragment>
	<svelte:fragment slot="sidebarRight">
		<div id="sidebar-right" class="hidden lg:block">Sidebar Right</div>
	</svelte:fragment>
	<svelte:fragment slot="pageHeader">
		
	</svelte:fragment>

	<div class="max-w-7xl mx-auto">
		<slot />
	</div>

	<svelte:fragment slot="pageFooter">

	</svelte:fragment>
	<svelte:fragment slot="footer">
		
	</svelte:fragment>
</AppShell>