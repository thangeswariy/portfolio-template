<template>
  <div class="flex flex-col w-screen h-full">
    <!-- Your name, profile picture and contact -->
    <HeadWrapper 
      name='Your Name'
      title='Your Job Title'
      userImgUrl='Image URL Address'
      phone='Your Contact Number'
      email='Your Email Contact'
    />
    <!-- About Me -->
    <AboutWrapper 
      aboutMe='Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.'
      linkedInURL='Your LinkedIn URL Address'
      languages='Languages'
      nationality='Your Nationality'
      interest='Your Interest'
    />
    <!-- Working Experience -->
    <CareerWrapper>
      <template v-slot:career>
        <Career 
          companyName='Company Name'
          title='Your Job Title'
          startDate='Start Date'
          endDate='End Date'
          >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class='text-gray-600 list-inside list-disc mt-2 px-4'>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>
        
        <Career 
          companyName='Company Name'
          title='Your Job Title'
          startDate='Start Date'
          endDate='End Date'
          >
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class='text-gray-600 list-inside list-disc mt-2 px-4'>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>
      </template>
    </CareerWrapper>
    <!-- Achievement -->
    <AchievementWrapper 
      project='Number of Project'
      client='Number of Happy Clients'
      award='Number of Awards'
    />
    <!-- Portfolio -->
    <PortfolioWrapper>
        <template v-slot:portfolio>
          <div class='grid grid-cols-1 md:grid-cols-3'>
            <ProjectCard 
              imgUrl='../img/github.png'
              name='Project Name'
              project='Project Type'
              projectURL='https://github.com'
              />

              <ProjectCard 
              imgUrl='../img/github.png'
              name='Project Name'
              project='Project Type'
              projectURL='https://github.com'
              />
              
              <ProjectCard 
              imgUrl='../img/github.png'
              name='Project Name'
              project='Project Type'
              projectURL='https://github.com'
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
      title: 'Your Name'
    }
  }
}
</script>