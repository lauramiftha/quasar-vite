<template>
    <q-page>
      <q-page-container>
        <div class="about-container">
          <h1>About Office Scheduler</h1>
          <p class="about-description">
            Office Scheduler is a powerful scheduling application designed to streamline and manage office tasks and
            appointments effectively. With Office Scheduler, you can easily schedule meetings, organize events, and track
            tasks, ensuring efficient collaboration and productivity in your workplace.
          </p>
          <div class="about-features">
            <h2>Key Features</h2>
            <ul>
              <li>Schedule and manage appointments</li>
              <li>Create and track tasks and deadlines</li>
              <li>Organize and notify team members about meetings and events</li>
              <li>Intuitive and user-friendly interface</li>
              <li>Real-time updates and notifications</li>
              <li>Flexible customization options</li>
            </ul>
          </div>
          <div class="about-team">
            <h2>Our Team</h2>
            <div class="team-members">
              <div class="team-member">
                <img src="https://example.com/path/to/avatar1.jpg" alt="Team Member 1" class="member-avatar" />
                <p class="member-name">John Doe</p>
                <p class="member-role">UI/UX Designer</p>
              </div>
              <div class="team-member">
                <img src="https://example.com/path/to/avatar2.jpg" alt="Team Member 2" class="member-avatar" />
                <p class="member-name">Jane Smith</p>
                <p class="member-role">Backend Developer</p>
              </div>
              <!-- Add more team members as needed -->
            </div>
          </div>
        </div>
      </q-page-container>
    </q-page>
  </template>
  
  <script>
  export default {
    name: "About",
  };
  </script>
  
  <style scoped>
  .about-container {
    margin: 20px;
  }
  
  h1 {
    font-size: 24px;
    font-weight: bold;
    color: #333;
    margin-bottom: 20px;
  }
  
  .about-description {
    font-size: 16px;
    color: #666;
    margin-bottom: 30px;
  }
  
  .about-features h2 {
    font-size: 20px;
    font-weight: bold;
    color: #333;
    margin-bottom: 10px;
  }
  
  .about-features ul {
    list-style-type: disc;
    margin-left: 20px;
    font-size: 16px;
    color: #666;
  }
  
  .about-team h2 {
    font-size: 20px;
    font-weight: bold;
    color: #333;
    margin-bottom: 10px;
  }
  
  .team-members {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  
  .team-member {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 200px;
  }
  
  .member-avatar {
    width: 100px;
    height: 100px;
    border-radius: 50%;
  }
  
  .member-name {
    font-size: 18px;
    font-weight: bold;
    color: #333;
    margin-top: 10px;
  }
  
  .member-role {
    font-size: 14px;
    color: #666;
    margin-top: 5px;
  }
  </style>
  
