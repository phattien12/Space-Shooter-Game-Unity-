<!-- ===================== HEADER ===================== -->
<h1 align="center">🚀 Space Shooter Game (Unity)</h1>

<p align="center">
  <b>CE318 / CE818 - High-level Games Development</b><br/>
  Lab 3 & Lab 4 Implementation
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Unity-3D-black?logo=unity">
  <img src="https://img.shields.io/badge/C%23-Scripting-blue?logo=csharp">
  <img src="https://img.shields.io/badge/Platform-PC%20%7C%20Web-green">
</p>

<hr/>

<!-- ===================== VIDEO DEMO ===================== -->
<h2>🎥 Demo Video</h2>

<p align="center">
  <a href="https://youtu.be/B8Dx5EMmOKk">
    <img src="https://img.youtube.com/vi/B8Dx5EMmOKk/0.jpg" alt="Watch the video" width="600"/>
  </a>
</p>

<p align="center">
  👉 Click the image above to watch the demo on YouTube
</p>

<hr/>

<!-- ===================== INTRO ===================== -->
<h2>📖 Introduction</h2>

<p>
This project is a <b>Space Shooter game</b> developed in Unity as part of the 
<b>CE318/CE818: High-level Games Development</b> course.
</p>

<p>
The game is based on the official Unity tutorial:
<br/>
<a href="https://unity3d.com/learn/tutorials/projects/space-shooter-tutorial">
Space Shooter Tutorial
</a>
</p>

<p>
The project is divided into two parts:
</p>

<ul>
  <li><b>Lab 3:</b> Core gameplay mechanics</li>
  <li><b>Lab 4:</b> Advanced features (audio, UI, scoring, camera animation)</li>
</ul>

<hr/>

<!-- ===================== FEATURES ===================== -->
<h2>🎮 Features</h2>

<style>
.feature-box {
  background-color: #f6f8fa;
  padding: 12px;
  border-radius: 8px;
  margin-bottom: 10px;
}
</style>

<div class="feature-box">
✔ Player movement with keyboard controls  
</div>

<div class="feature-box">
✔ Shooting system with cooldown  
</div>

<div class="feature-box">
✔ Asteroid spawning (wave system using Coroutine)  
</div>

<div class="feature-box">
✔ Collision detection & destruction  
</div>

<div class="feature-box">
✔ Explosion effects (VFX prefabs)  
</div>

<div class="feature-box">
✔ Background music & sound effects  
</div>

<div class="feature-box">
✔ Score system & UI display  
</div>

<div class="feature-box">
✔ Game Over & Restart functionality  
</div>

<div class="feature-box">
✔ Camera intro cutscene animation  
</div>

<hr/>

<!-- ===================== GAMEPLAY ===================== -->
<h2>🕹️ Gameplay</h2>

<table>
<tr><th>Action</th><th>Control</th></tr>
<tr><td>Move</td><td>Arrow Keys</td></tr>
<tr><td>Shoot</td><td>Custom key (e.g. Space)</td></tr>
<tr><td>Restart</td><td>S</td></tr>
</table>

<hr/>

<!-- ===================== PROJECT STRUCTURE ===================== -->
<h2>📂 Project Structure</h2>

<pre>
Assets/
│
├── Models/
├── Prefabs/
│   ├── VFX/
│   └── Asteroids/
│
├── Scripts/
│   ├── PlayerController.cs
│   ├── BoltController.cs
│   ├── DestroyByBoundary.cs
│   ├── DestroyByContact.cs
│   ├── GameController.cs
│   ├── DestroyByTime.cs
│   ├── Mover.cs
│   └── RandomRotator.cs
│
├── Audio/
├── Textures/
└── Scenes/
</pre>

<hr/>

<!-- ===================== IMPLEMENTATION ===================== -->
<h2>⚙️ Implementation Details</h2>

<h3>1. Player</h3>
<ul>
  <li>Uses <b>Rigidbody</b> (no gravity)</li>
  <li>Movement constrained within screen bounds</li>
  <li>Tilts based on horizontal velocity</li>
</ul>

<h3>2. Shooting System</h3>
<ul>
  <li>Instantiates bolt prefabs</li>
  <li>Uses cooldown timer</li>
  <li>Audio triggered when shooting</li>
</ul>

<h3>3. Asteroids (Hazards)</h3>
<ul>
  <li>Random rotation using angular velocity</li>
  <li>Moves toward player</li>
  <li>Destroyed on collision</li>
</ul>

<h3>4. Spawning System</h3>
<ul>
  <li>Implemented using <b>Coroutine</b></li>
  <li>Spawns waves with delay</li>
</ul>

<h3>5. Boundary System</h3>
<ul>
  <li>Destroys objects leaving game area</li>
</ul>

<h3>6. Explosion Effects</h3>
<ul>
  <li>Asteroid explosion</li>
  <li>Player explosion</li>
  <li>Auto-destroy after time</li>
</ul>

<h3>7. Game Controller</h3>
<ul>
  <li>Handles score</li>
  <li>Spawns waves</li>
  <li>Controls game state</li>
</ul>

<h3>8. UI System</h3>
<ul>
  <li>Score display (bottom-right)</li>
  <li>Game Over message (center)</li>
  <li>Restart instruction (top-left)</li>
</ul>

<h3>9. Audio</h3>
<ul>
  <li>Background music (looped)</li>
  <li>Explosion sounds</li>
  <li>Shooting sound</li>
</ul>

<h3>10. Camera Animation</h3>
<ul>
  <li>Intro cutscene</li>
  <li>Smooth transition to gameplay view</li>
</ul>

<hr/>

<!-- ===================== BUILD ===================== -->
<h2>🛠️ Build Instructions</h2>

<ol>
  <li>Open Unity Project</li>
  <li>Go to <b>File → Build Settings</b></li>
  <li>Select <b>PC Platform</b></li>
  <li>Click <b>Add Current Scene</b></li>
  <li>Click <b>Build</b></li>
</ol>

<p>
After building, run the generated <b>.exe</b> file to play the game.
</p>

<hr/>

<!-- ===================== REQUIREMENTS ===================== -->
<h2>📋 Requirements</h2>

<ul>
  <li>Unity (recommended version: 5.x or later)</li>
  <li>C# scripting knowledge</li>
</ul>

<hr/>

<!-- ===================== AUTHOR ===================== -->
<h2>👨‍💻 Author</h2>

<p>
<b>Name:</b> Phat  
<br/>
<b>Course:</b> CE318 / CE818  
</p>

<hr/>

<!-- ===================== FOOTER ===================== -->
<p align="center">
  ⭐ If you like this project, consider giving it a star!
</p>