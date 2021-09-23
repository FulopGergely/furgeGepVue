<template>
  <div class="gepkolcsonzes">
    <Gyalu msg="Welcome to Your Gyalu" />
  </div>
</template>


<script>
// @ is an alias to /src
import Gyalu from "@/components/Gyalu.vue";

export default {
  name: "gyalu",
  components: {
    Gyalu,
  },
};
</script>
