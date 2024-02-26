<script lang="ts">
	import Icon from '@iconify/svelte'

  export let icon, style = '', title = '', big = false, double = false, rot180 = false, cls
</script>

<i {style} {title} class:big class:double class:rot180 class={cls}><Icon {icon}/></i>

<style>
	i {
    width : var(--size, 1em);
    height: var(--size, 1em);
		display: inline-flex;
		align-items: center;
		justify-content: center;
    flex-shrink: 0;
	}
	i.big {
		font-size: 1.5em;
	}
	i.double {
		font-size: 2em;
	}
	i.rot180 {
		transform: rotate(180deg);
	}
</style>
