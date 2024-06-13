<template>
    <div class="admin-dashboard">
        <!-- Sidebar -->
        <div class="sidebar">
            <div class="logo">
                <img src="logo.png" alt="Logo" class="logo-img">
            </div>
            <div class="menu">
                <router-link to="/home">Home</router-link>
                <router-link to="/profile">Profile</router-link>
                <router-link to="/settings">Settings</router-link>
            </div>
        </div>
        <!-- Main Content -->
        <div class="main-content">
            <div class="header">
                <h2>Dashboard</h2>
            </div>
            <div class="content">
                <!-- Your main content goes here -->
            </div>
        </div>
    </div>
</template>

<style scoped>
/* General styling */
.admin-dashboard {
    display: flex;
    min-height: 100vh;
}

/* Sidebar */
.sidebar {
    width: 250px;
    background-color: #2c3e50;
    color: white;
    padding: 20px;
}

.logo {
    text-align: center;
    margin-bottom: 20px;
}

.logo-img {
    width: 80%;
}

.menu {
    display: flex;
    flex-direction: column;
}

.menu router-link {
    color: #fff;
    text-decoration: none;
    margin-bottom: 10px;
    padding: 10px;
    transition: background-color 0.3s ease;
}

.menu router-link:hover {
    background-color: #34495e;
}

/* Main Content */
.main-content {
    flex: 1;
    display: flex;
    flex-direction: column;
    background-color: #ecf0f1;
    padding: 20px;
    border-left: 1px solid #ddd; /* Add a border for separation */
}

.header {
    background-color: #34495e;
    color: white;
    padding: 20px;
    border-bottom: 1px solid #ddd; /* Add a border for separation */
}

.content {
    flex: 1;
    overflow-y: auto;
}

.content h2 {
    margin-bottom: 20px;
}
</style>
