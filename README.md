/* Created by Dipika Sharma */

body {
    font-family: Arial;
    margin: 0;
    background: #f5f5f5;
}

/* Header */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #0c8f3f;
    color: white;
    padding: 15px;
}

.logo {
    font-size: 22px;
    font-weight: bold;
}

header input {
    width: 40%;
    padding: 8px;
    border-radius: 5px;
    border: none;
}

/* Products */
.section-title {
    padding: 15px;
}

.container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 15px;
    padding: 20px;
}

.card {
    background: white;
    padding: 10px;
    border-radius: 10px;
    text-align: center;
    transition: 0.3s;
}

.card:hover {
    transform: scale(1.05);
}

.card img {
    width: 100%;
    height: 120px;
    object-fit: cover;
}

button {
    background: #0c8f3f;
    color: white;
    border: none;
    padding: 8px;
    margin-top: 5px;
    cursor: pointer;
    border-radius: 5px;
}

/* Portfolio */
.portfolio {
    background: white;
    margin: 20px;
    padding: 20px;
    border-radius: 10px;
}

.profile {
    display: flex;
    align-items: center;
    gap: 20px;
}

.profile img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
}

/* Links */C:\Users\M S I\OneDrive\Desktop
.links a {
    background: #0c8f3f;
    color: white;
    padding: 8px 12px;
    margin-right: 10px;
    text-decoration: none;
    border-radius: 5px;
}

/* Footer */
footer {
    background: #222;
    color: white;
    text-align: center;
    padding: 10px;
}
