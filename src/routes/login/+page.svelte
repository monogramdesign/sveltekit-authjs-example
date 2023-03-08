<script lang="ts">
  import { page } from '$app/stores'
  import { signIn, signOut } from '@auth/sveltekit/client'
</script>

{#if !$page.data.session}
  <button on:click={() => signIn('github', { callbackUrl: '/' })}>
    Sign in with GitHub
  </button>
{:else}
  <button on:click={signOut}> Log out</button>
{/if}
