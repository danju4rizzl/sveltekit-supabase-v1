<script lang="ts">
import "../app.css";

/**
 * TODO: Remove the greetUser function  and clean the page
 */
const d = new  Date()

const greetUser = (time: number) => `Good ${time < 12 ? 'Morning' : time < 18 ? 'Afternoon' : 'Evening'}, Dev's 👋`;

const currentHour = d.getHours()

</script>

<!-- Navbar -->

<div class="p-5 text-center">
  <h1 class="text-xl ">{greetUser(currentHour)}</h1>
</div>

<slot></slot>
