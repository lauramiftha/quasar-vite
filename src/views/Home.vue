<template>
    <q-page>
      <q-page-container>
        <div class="header">
          <h1 class="app-title">Welcome to Office Scheduling App</h1>
        </div>
  
        <div class="navigation">
          <router-link to="/about">Go to About Page</router-link>
        </div>
  
        <!-- Today's Schedule -->
        <div class="layout">
          <h2 class="section-title">Today's Schedule</h2>
          <div class="schedule-list">
            <div class="schedule">
              <i class="fas fa-calendar-alt"></i>
              <div class="schedule-details">
                <p class="schedule-title">Meeting</p>
                <p class="schedule-time">10:00 AM - 11:00 AM</p>
              </div>
            </div>
            <!-- Add more schedule items as needed -->
          </div>
        </div>
  
        <!-- Upcoming Events -->
        <div class="layout">
          <h2 class="section-title">Upcoming Events</h2>
          <div class="event-list">
            <div class="event">
              <i class="fas fa-briefcase"></i>
              <div class="event-details">
                <p class="event-title">Conference</p>
                <p class="event-time">May 29, 9:00 AM - 5:00 PM</p>
              </div>
            </div>
            <!-- Add more events as needed -->
          </div>
        </div>
  
        <!-- Useful Features -->
        <div class="layout">
          <h2 class="section-title">Useful Features</h2>
          <ul class="feature-list">
            <li class="feature">
              <i class="fas fa-check"></i>
              <p class="feature-description">Schedule and manage appointments</p>
            </li>
            <li class="feature">
              <i class="fas fa-check"></i>
              <p class="feature-description">Create and track tasks and deadlines</p>
            </li>
            <li class="feature">
              <i class="fas fa-check"></i>
              <p class="feature-description">Organize and notify team members about meetings and events</p>
            </li>
            <li class="feature">
              <i class="fas fa-check"></i>
              <p class="feature-description">Intuitive and user-friendly interface</p>
            </li>
            <li class="feature">
              <i class="fas fa-check"></i>
              <p class="feature-description">Real-time updates and notifications</p>
            </li>
            <li class="feature">
              <i class="fas fa-check"></i>
              <p class="feature-description">Flexible customization options</p>
            </li>
          </ul>
        </div>
      </q-page-container>
    </q-page>
  </template>
  
  <script>
  export default {
    name: "Home",
  };
  </script>
  
  <style scoped>
  .header {
    background-color: #f5f5f5;
    padding: 20px;
    text-align: center;
  }
  
  .app-title {
    font-size: 32px;
    font-weight: bold;
    color: #333;
    margin-bottom: 10px;
  }
  
  .navigation {
    display: flex;
    justify-content: center;
    margin-bottom: 20px;
  }
  
  .navigation a {
    color: #333;
    text-decoration: none;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  .layout {
    margin: 20px;
    padding: 10px;
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .section-title {
    font-size: 24px;
    font-weight: bold;
    color: #333;
    margin-bottom: 10px;
    padding-bottom: 5px;
    border-bottom: 1px solid #ccc;
  }
  
  .schedule-list,
  .event-list {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 20px;
  }
  
  .schedule,
  .event {
    display: flex;
    align-items: center;
    padding: 10px;
    background-color: #f9f9f9;
    border-radius: 4px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .schedule i,
  .event i {
    font-size: 24px;
    color: #888;
    margin-right: 10px;
  }
  
  .schedule-details,
  .event-details {
    flex: 1;
  }
  
  .schedule-title,
  .event-title {
    font-weight: bold;
    font-size: 18px;
    color: #333;
    margin: 0;
  }
  
  .schedule-time,
  .event-time {
    font-size: 14px;
    color: #666;
    margin: 0;
  }
  
  .feature-list {
    list-style-type: none;
    padding-left: 0;
    margin-top: 20px;
  }
  
  .feature {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  
  .feature i {
    font-size: 16px;
    color: #2ecc71;
    margin-right: 10px;
  }
  
  .feature-description {
    font-size: 16px;
    color: #333;
    margin: 0;
  }
  </style>
  
   