<template>
  <section id="skill" class="fade-in">
    <p class="text-[50px]">Skills</p>
    <div class="skill-gallery gap-4">
      <div>
        <p class="skill-header skill-devops">Devops</p>
        <div class="flex px-3 py-10 bg-white rounded-lg justify-around gap-2">
          <img class="skill devops-1" src="../assets/skills/nginx.png" />
          <img class="skill devops-2" src="../assets/skills/aws.png" />
          <img class="skill devops-3" src="../assets/skills/digital_ocean.png" />
        </div>
      </div>
      <div>
        <p class="skill-header skill-frontend">Frontend</p>
        <div class="flex px-3 py-10 bg-white rounded-lg justify-around gap-2">
          <img class="skill frontend-1" src="../assets/skills/vue.png" />
          <img class="skill frontend-2" src="../assets/skills/html.png" />
          <img class="skill frontend-3" src="../assets/skills/css.webp" />
        </div>
      </div>
      <div>
        <p class="skill-header skill-backend">Backend</p>
        <div class="flex px-3 py-10 bg-white rounded-lg justify-around gap-2">
          <img class="skill backend-1" src="../assets/skills/node.png" />
          <img class="skill backend-2" src="../assets/skills/express.png" />
        </div>
      </div>
      <div>
        <p class="skill-header skill-database">Database</p>
        <div class="flex px-3 py-10 bg-white rounded-lg justify-around gap-2">
          <img class="skill database-1" src="../assets/skills/mysql.png" />
          <img class="skill database-2" src="../assets/skills/postgresql.webp" />
        </div>
      </div>
      <div class="col-span-full">
        <p class="skill-header skill-knowledge">Knowledges</p>
        <div class="flex flex-wrap px-3 py-10 bg-white rounded-lg justify-around gap-6">
          <img class="skill knowledge knowledge-1" src="../assets/skills/javascript.png" />
          <img class="skill knowledge knowledge-2" src="../assets/skills/typescript.png" />
          <img class="skill knowledge knowledge-3" src="../assets/skills/python.png" />
          <img class="skill knowledge knowledge-4" src="../assets/skills/git.png" />
          <img class="skill knowledge knowledge-5" src="../assets/skills/microservice.png" />
          <img class="skill knowledge knowledge-6" src="../assets/skills/docker.png" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.skill-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(min(100%, 350px), 1fr));
}

.skill-gallery > div {
  padding: 2rem 1rem;
  border-radius: 20px;
  background: #ececf1;
}

.skill-header {
  font-size: 32px;
}

.skill-header::after {
  content: '';
  font-size: 30px;
  opacity: 0;
  transition: opacity 300ms ease-out;
}

.skill-devops:has(+ div > .devops-1:hover)::after {
  content: ': nginx';
}

.skill-devops:has(+ div > .devops-2:hover)::after {
  content: ': aws';
}

.skill-devops:has(+ div > .devops-3:hover)::after {
  content: ': digital ocean';
}

.skill-frontend:has(+ div > .frontend-1:hover)::after {
  content: ': vue';
}

.skill-frontend:has(+ div > .frontend-2:hover)::after {
  content: ': html';
}

.skill-frontend:has(+ div > .frontend-3:hover)::after {
  content: ': css';
}

.skill-backend:has(+ div > .backend-1:hover)::after {
  content: ': node';
}

.skill-backend:has(+ div > .backend-2:hover)::after {
  content: ': express';
}

.skill-database:has(+ div > .database-1:hover)::after {
  content: ': mysql';
}

.skill-database:has(+ div > .database-2:hover)::after {
  content: ': postgresql';
}

.skill-knowledge:has(+ div > .knowledge-1:hover)::after {
  content: ': javascript';
}

.skill-knowledge:has(+ div > .knowledge-2:hover)::after {
  content: ': typescript';
}

.skill-knowledge:has(+ div > .knowledge-3:hover)::after {
  content: ': python';
}

.skill-knowledge:has(+ div > .knowledge-4:hover)::after {
  content: ': git';
}

.skill-knowledge:has(+ div > .knowledge-5:hover)::after {
  content: ': microservice';
}

.skill-knowledge:has(+ div > .knowledge-6:hover)::after {
  content: ': docker';
}

.skill-header:has(+ div > .skill:hover)::after {
  opacity: 1;
}

.knowledge {
  flex-basis: 110px;
}

@media (min-width: 480px) {
  .knowledge {
    flex-basis: 160px;
  }
}

@media (min-width: 768px) {
  .knowledge {
    flex-basis: 60px;
  }
}

.skill {
  max-height: 60px;
  object-fit: contain;
  transition: scale 250ms ease-out;
}

.skill:hover {
  scale: 1.4;
}
</style>