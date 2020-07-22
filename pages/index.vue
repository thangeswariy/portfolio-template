<template>
  <div class="flex flex-col w-screen h-full">
    <!-- Your name, profile picture and contact -->
    <HeadWrapper
      name="Thangeswariy"
      title="Full Stack Developer"
      userImgURL="../img/Thangeswariy.png"
      phone="012-4961629"
      email="thangeswariyramanei@gmail.com"
    />
    <!-- About Me -->
    <AboutWrapper
      aboutMe="Solution creator|Data Scientist."
      linkedInURL="https://www.linkedin.com/in/thangeswariyramanei/"
      languages="English, Malay, Tamil"
      nationality="Malaysian"
      interest="Classical music string instrument"
    />
    <!-- Working Experience -->
    <CareerWrapper>
      <template v-slot:career>
        <Career
          companyName="Sony EMCS PG Tec Sdn Bhd"
          title="Senior Executive"
          startDate="1st Apr 2019"
          endDate="30th June 2020"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Order Management.</li>
              <li>Effective communication with logistics and production planners.</li>
              <li>Implementation of cumulative approach to minimize excess parts.</li>
            </ul>
          </template>
        </Career>

        <Career
          companyName="Sony EMCS PG TEC Sdn Bhd"
          title="Executive"
          startDate="19th December 2016"
          endDate="31st March 2019"
        >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>97% standard DS achieved.</li>
              <li>advance shipment</li>
              <li>data integration for P & L report.</li>
            </ul>
          </template>
        </Career>
      </template>
    </CareerWrapper>
    <!-- Achievement -->
    <AchievementWrapper project="6" client="6" award="6"/>
    <!-- Portfolio -->
    <PortfolioWrapper>
      <template v-slot:portfolio>
        <div class="grid grid-cols-1 md:grid-cols-3">
          <ProjectCard
            imgUrl="../img/thangeswariy.png"
            name="My portfolio"
            project="Project Mission"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />
        </div>
      </template>
    </PortfolioWrapper>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Thangeswariy"
    };
  }
};
</script>