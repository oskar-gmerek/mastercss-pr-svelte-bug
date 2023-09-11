<script lang="ts">
    import { onMount, type ComponentType } from "svelte";
    import { Fragment } from "@master/css.svelte";
    import type { CSSProvider as CSSProviderType } from "@master/css.svelte";
 
    let CSSProvider: ComponentType<CSSProviderType> = Fragment as any;
 
    onMount(async () => {
        CSSProvider = (await import("@master/css.svelte")).CSSProvider;
    });
</script>
 <svelte:component this={CSSProvider} config={import('../master.css')}>
 <!-- <CSSProvider config={import("../master.css")}> -->
    <div class="fg:black bg:green-70 h:full w:full min-h:100vh min-w:100vw">
        <slot />
    </div>
<!-- </CSSProvider> -->
</svelte:component>