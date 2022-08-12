<template>
  <div class="container">
    <h2>About Me</h2>
    <p>
Hi! My Name is Anik Chandra.I'm a Developer, Programmer and aslo a blogger,and I'm very passionate and dedicated to my work.
With 4 years academic experience as a various skills such as CP, devlopment,Machine learnging etc.I have acquired the skills and knowledge necessary to make my project a success.
I enjoy every step of the solveing process,from discussion and collaboration
    </p>
    <h4>My Skills</h4>
    <div v-for="skill in skillProgress" :key="skill">
      <h6>{{ skill.title }}</h6>
      <div class="progress">
        <div
          class="progress-bar bg-success"
          role="progressbar"
          :aria-valuenow="`${skill.vNow}`"
          aria-valuemin="0"
          aria-valuemax="100"
          :style="{ width: skill.vStyle }"
        ></div>
      </div>
    </div>
    <h4>My Resume:</h4>
    <p>
      Hi! My Name is Anik Chandra.I'm a Developer, Programmer and aslo a blogger, and I'm very passionate and dedicated to my work.
    </p>
    <a href="#" class="btn btn-warning mt-2 mb-3">Download My Resume</a>
  </div>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      // define my Skills
      skillProgress: [
        { title: "Html:", vNow: 70, vStyle: "70%" },
        { title: "Css:", vNow: 60, vStyle: "60%" },
        { title: "Bootstrap:", vNow: 65, vStyle: "65%" },
        { title: "Javascript:", vNow: 60, vStyle: "60%" },
        { title: "Vuejs:", vNow: 40, vStyle: "40%" },
        { title: "Python:", vNow: 70, vStyle: "70%" },
        { title: "Django:", vNow: 60, vStyle: "60%" },
      ],
    };
  },
};
</script>

<style scoped>
h6 {
  margin: 1rem 0;
}
</style>
