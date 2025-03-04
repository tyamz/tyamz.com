<script setup lang="ts"></script>
<template>
  <header>
    <div class="logo-container">
      <img alt="TYAMZ logo" class="logo" src="../assets/tyamz-full.svg" />
    </div>
    <span class="slogan">Thomas Yamakaitis</span>
    <span class="under-slogan">Senior Software Engineer</span>
  </header>
  <main>
    <h2>About Me</h2>
    <div class="about">
      <p>
        My name is Thomas Yamakaitis, and I was born and raised in New Jersey. With over five years
        of experience in software engineering, I am a highly skilled and innovative professional at
        The Compuflex Corporation, where I have been leading critical projects and driving
        technological advancements since 2018. As a Lead Engineer, I have successfully designed and
        develop many solutions using many of the technologies listed below.
      </p>
      <p>
        My greatest achievement at Compuflex being system design and development of the universal
        cash integration solution which extended the company's flagship integration product with a
        WebSocket interface using a combination of C#, TypeScript, React and Java. This product
        reduces installation overhead by nearly 80% for large institutions looking for a direct
        integration with Cash Recyclers.
      </p>
      <p>
        Another notable accomplishment was my design and implementation of a backroom till
        management solution which enabled retail clients to reduce theft, dual entry and user error
        while prcessing start and end funds for cashiers. This product allows for less personnel
        on-site and frees up a member of management who would normally need to manually count a
        start fund for a cashier's shift or rely on an unreliable cash counting device. This project
        was implemented using C#, TypeScript, React and Electron.
      </p>
      <ul>
        <li>Education: B.S. in Computer Science from Kean University; GPA: 3.558</li>
        <li>Skills: Languages: JavaScript / TypeScript, C# / .NET, Java, PHP, SQL, HTML</li>
        <li>Frameworks / Libraries: Node.js, React, Electron / Vite.js, Laravel / OctoberCMS</li>
        <li>Technologies: REST, HTTP, APIs, WebSockets / SignalR, TCP</li>
        <li>Databases: MySQL, MSSQL, Postgres, SQLite, MongoDB, AmazonRDS, DynamoDB</li>
      </ul>
      <p>
        I am a strong advocate for knowledge sharing and have fostered a supportive environment for
        new team members, expediting onboarding time and ensuring a seamless transition into the
        team. My strategic approach to DevOps has enabled faster project delivery and compliance
        with technical requirements for major software releases. Additionally, my commitment to
        delivering critical updates on time has ensured SLA compliance for key clients, including
        major financial institutions.
      </p>
      <p>
        During my internship at The Compuflex Corporation, I modernized the company's website and
        collaborated on various projects, laying a solid foundation for my career in software
        development.
      </p>
      <p>
        Outside of my professional role, I have demonstrated my entrepreneurial spirit through
        contract work by designing and developing a custom e-commerce solution for the Jersey Cat
        Cafe, integrating the PayPal API and utilizing AWS Lambda for serverless operations.
      </p>
      <p>
        For another contract, I also designed and developed SurvElect, a robust voter database
        solution, leveraging cloud-based services to reduce campaign costs.
      </p>
      <p>
        With a proven track record of innovation, leadership, and technical excellence, I continue
        to thrive in the ever-evolving field of software engineering, always eager to embrace new
        challenges and drive meaningful change.
      </p>
    </div>
  </main>
</template>

<style scoped>
header {
  margin-top: 1rem;
}
main {
  margin: 0 auto;
  padding-bottom: 5rem;
}

.about {
  font-family: 'Teko', sans-serif;
  padding: 1rem;
  font-size: 1.2rem;
  color: #fff;
  background-color: #333;
  width: 80rem;
}

p {
  margin: 0;
}

@media (max-width: 1024px) {
  .logo {
    width: 250px;
    height: 50px;
  }
  .about {
    display: block;
    width: 20rem;
    max-height: 38rem;
    overflow-y: scroll;
  }
}
</style>
