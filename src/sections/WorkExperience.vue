<template>
  <section id="work" class="fade-in">
    <p class="text-[50px]">Work Experiences</p>
    <div class="grid md:grid-cols-[max-content,1fr] work gap-x-10">
      <div class="md:!p-10 md:!pl-0 md:border-r border-gray-400">
        <p class="text-[32px] md:text-right text-gray-400 timestamp">Since Jun 2024</p>
      </div>
      <div class="border-b border-gray-400">
        <p class="text-[32px]">Python Backend Developer</p>
        <p class="text-[24px] text-gray-400 mb-4">at Brainergy Digital</p>
        <p class="text-[20px]">Working on the e-tax & e-receipt system in backend role using Django with PostgreSQL database.</p>
      </div>

      <div class="md:!p-10 md:!pl-0 md:border-r border-gray-400">
        <p class="text-[32px] md:text-right text-gray-400 timestamp">Sep 2022 - May 2024</p>
      </div>
      <div class="border-b border-gray-400">
        <p class="text-[32px]">Fullstack developer</p>
        <p class="text-[24px] text-gray-400 mb-4">at House of Dev Technology</p>
        <p class="text-[20px]">Working on the company's ERP and customer products mainly in backend role using Node.js with MySQL and PostgreSQL database.</p>
      </div>

      <div class="md:!p-10 md:!pl-0 md:border-r border-gray-400">
        <p class="text-[32px] md:text-right text-gray-400 timestamp">Apr 2022</p>
      </div>
      <div class="border-b border-gray-400">
        <p class="text-[32px]">Algorithm Design Teacher Assistant</p>
        <p class="text-[24px] text-gray-400 mb-4">at Samsen Computer POSN 2</p>
        <p class="text-[20px]"></p>
      </div>

      <div class="md:!p-10 md:!pl-0 md:border-r border-gray-400">
        <p class="text-[32px] md:text-right text-gray-400 timestamp">2021 - 2022</p>
      </div>
      <div class="border-b border-gray-400">
        <p class="text-[32px]">Intern Backend Developer</p>
        <p class="text-[24px] text-gray-400 mb-4">at House of Dev Technology</p>
        <p class="text-[20px]">Worked with HOD UX/UI design team to create eLearning platform, capstone project.</p>
      </div>

      <div class="md:!p-10 md:!pl-0 md:border-r border-gray-400">
        <p class="text-[32px] md:text-right text-gray-400 timestamp">Apr - Jun 2021</p>
      </div>
      <div class="border-b border-gray-400">
        <p class="text-[32px]">Intern System Engineer</p>
        <p class="text-[24px] text-gray-400 mb-4">at KMUT North Bangkok</p>
        <p class="text-[20px] mb-2">Studied in Microservice and FaaS Architecture and worked on the vHive open-source framework for serverless architecture project.</p>
        <p class="text-[20px]">Our task is to setup, deploy and evaluate performance vHive using Kubernetes, Golang, Firecracker and Containerd.</p>
      </div>

      <div class="md:!p-10 md:!pl-0 md:border-r border-gray-400">
        <p class="text-[32px] md:text-right text-gray-400 timestamp">2020</p>
      </div>
      <div>
        <p class="text-[32px]">Algorithm Design Teacher Assistant</p>
        <p class="text-[24px] text-gray-400 mb-4">at University of Chulalongkorn</p>
        <p class="text-[20px]"></p>
      </div>
    </div>
  </section>
</template>

<style scoped>
.timestamp {
  position: relative;
}

.timestamp::after {
  position: absolute;
  content: '';
  background-color: red;
  border-radius: 100%;
  width: 16px;
  height: 16px;
  right: 100%;
  top: 50%;
  translate: -50% -50%;
}

.work > *:nth-child(odd) {
  padding-left: 1rem;
  padding-top: 2.5rem;
}

.work > *:nth-child(even) {
  padding-bottom: 2.5rem;
}

@media (min-width: 768px) {
  .work > * {
    padding: 2.5rem 0;
  }
  .timestamp::after {
    right: 0;
    translate: calc(50% + 2.5rem) -50%;
  }
}
</style>