<script lang="ts">
  import { page } from '$app/stores'
</script>

<h1>Welcome {$page.data.session?.user?.name}</h1>
<img
  width="200"
  src={$page.data.session?.user?.image}
  alt="github profile avatar"
/>
