<template>
<div>
  <div v-for="post in posts" :key="post.uuid">
    <h3>{{ post.title }}</h3>
    <h4>{{ post.description }}</h4>
    <p>{{ post.content }}</p>
  </div>
</div>
</template>

<script>
export default {
  name: "PostBloc",
  data() {
    return {
      posts: [
        {
          uuid: "1",
          title: "post número uno",
          description:
            "Descripción uno, Lorem ipsum dolor sit amet, consectetur adipiscing elit",
          content:
            "Contenido uno, Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        },
        {
          uuid: "2",
          title: "post número dos",
          description:
            "Descripción dos, Lorem ipsum dolor sit amet, consectetur adipiscing elit",
          content:
            "Contenido dos, Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        },
        {
          uuid: "3",
          title: "post número tres",
          description:
            "Descripción tres, Lorem ipsum dolor sit amet, consectetur adipiscing elit",
          content:
            "Contenido tres, Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        },
      ],
    };
  },
  components: {},
};
</script>

<style></style>
