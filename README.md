<div align="center">

  <div style="background-color: #0d1117; border: 1px solid #30363d; border-radius: 14px; padding: 36px 20px; text-align: center; font-family: 'Segoe UI', system-ui, sans-serif;">
  <h1 style="color: #00ff00; font-size: 52px; font-weight: 800; letter-spacing: 3px; margin: 0 0 14px 0;">
    ASIF AHMED
  </h1>
  <p style="color: #a259ff; font-family: 'Fira Code', Consolas, monospace; font-size: 15px; font-weight: 600; letter-spacing: 1.5px; margin: 0;">
    [ GAME DEVELOPER &nbsp;//&nbsp; MULTIPLAYER ] &amp; GRAPHICS PROGRAMMER
  </p>
</div>

 <br>
  
</div>


<pre>
${\color{#00ff41}\texttt{Primary\_Role\ \ :\ Game\ Developer\ \&\ Multiplayer\ Systems\ Engineer}}$
${\color{#00ff41}\texttt{Language\ \ \ \ \ \ :\ [\ C\#,\ C,\ HLSL\ /\ CG\ ]}}$
${\color{#00ff41}\texttt{Engines/APIs\ \ :\ [\ Unity,\ PurrNet,\ SDL2,\ Win32\ API\ ]}}$
${\color{#00ff41}\texttt{3D\_Pipeline\ \ \ :\ [\ Blender,\ ProBuilder\ ]}}$
${\color{#00ff41}\texttt{Build\_Targets\ :\ [\ Windows\ (x64),\ Android\ (ARM64),\ WebGL\ ]}}$
${\color{#00ff41}\texttt{Contact\ \ \ \ \ \ \ :\ asifahmed9510@gmail.com}}$
</pre>




<!-- SECTION 01 & 02: OVERVIEW & TECH STACK -->
<table width="100%">
  <tr>
    <td width="55%" valign="top">
      <h3>01 // SYSTEM OVERVIEW</h3>
      <p>
        I am a self-driven <b>Game Developer</b> and <b>Software Engineer</b> focused on building high-performance multiplayer systems, responsive character controllers, and low-level interactive applications.
      </p>
      <p>
        My approach to development is hands-on. Whether I am debugging RPC packet flow in <b>PurrNet</b>, writing custom <b>HLSL skybox shaders</b> in Unity URP, rigging 3D character meshes in <b>Blender</b>, or writing raw event loops from scratch in <b>C and SDL2</b>.
      </p>
      <p>
        Good Frame times, clean memory management, rapid iteration workflows, and making gameplay mechanics feel tight and immediate across both local and networked environments is my priority.
      </p>
    </td>
    <td width="45%" valign="top">
      <h3>02 // TECHNICAL ARSENAL</h3>
      <p>
        <b>Languages & Shading</b><br />
        <img src="https://img.shields.io/badge/C%23-181717?style=flat-square&logo=csharp&logoColor=a259ff" />
        <img src="https://img.shields.io/badge/C_Language-181717?style=flat-square&logo=c&logoColor=a259ff" />
        <img src="https://img.shields.io/badge/HLSL_%2F_CG-181717?style=flat-square&logoColor=a259ff" />
        <img src="https://img.shields.io/badge/JSON_Serialization-181717?style=flat-square" />
      </p>
      <p>
        <b>Engines, Networking & Native APIs</b><br />
        <img src="https://img.shields.io/badge/Unity_Engine-181717?style=flat-square&logo=unity&logoColor=white" />
        <img src="https://img.shields.io/badge/Universal_Render_Pipeline_(URP)-181717?style=flat-square" />
        <img src="https://img.shields.io/badge/PurrNet_Multiplayer-a259ff?style=flat-square" />
        <img src="https://img.shields.io/badge/SDL2-181717?style=flat-square&logo=sdl&logoColor=white" />
        <img src="https://img.shields.io/badge/Win32_API_(windows.h)-181717?style=flat-square" />
      </p>
      <p>
        <b>3D Modeling, Rigging & Level Design</b><br />
        <img src="https://img.shields.io/badge/Blender_3D-181717?style=flat-square&logo=blender&logoColor=F5792A" />
        <img src="https://img.shields.io/badge/ProBuilder_CSG-181717?style=flat-square" />
        <img src="https://img.shields.io/badge/Animation_Rigging_%2F_IK-181717?style=flat-square" />
        <img src="https://img.shields.io/badge/NavMesh_%26_A*_Pathfinding-181717?style=flat-square" />
      </p>
    </td>
  </tr>
</table>

<br />

<!-- SECTION 03: MULTIPLAYER & NETWORKING -->
<h3>03 // MULTIPLAYER & NETWORKING ARCHITECTURE (PURRNET & UNITY)</h3>
<p>
  Designing multiplayer games requires balancing responsiveness with authority. My networking work centers around <b>PurrNet</b> and custom peer-to-peer implementations in Unity, focusing on bandwidth efficiency and rapid multi-client testing.
</p>

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h4>PurrNet Framework Mastery</h4>
      <ul>
        <li><b>RPC Architecture:</b> Extensive implementation of static and generic Remote Procedure Calls (RPCs) for low-overhead cross-client communication and modular gameplay events.</li>
        <li><b>Networked Character Controllers:</b> Built synchronized First-Person (FPS) and Third-Person (TPS) controllers featuring smooth transform interpolation, networked crouching, and procedural ledge-climbing.</li>
        <li><b>State & Inventory Synchronization:</b> Engineered real-time inventory hotbar cycling and weapon state syncing across connected peers without desyncs.</li>
        <li><b>Bandwidth-Conscious Visuals:</b> Separated critical networked combat state (raycast hit detection, health synchronization) from heavy client-side effects—such as spawning localized blood decals and impact particles purely on the receiving client to keep packet sizes minimal.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h4>Custom P2P & Session Engineering</h4>
      <ul>
        <li><b>Peer-to-Peer Matchmaking:</b> Designed custom P2P lobby and matchmaking pipelines using unique session ID generation, direct local hosting, and client connection validation.</li>
        <li><b>JSON Player State Tracking:</b> Built lightweight serialization layers using JSON to track persistent player metadata, session states, and loadout configurations across matches.</li>
        <li><b>Networked World Streaming:</b> Integrated multiplayer session handlers with Unity's additive scene loading to stream large terrains seamlessly while maintaining active network identities.</li>
        <li><b>Fast-Iteration Netcode Workflow:</b> Configured rapid Mono scripting backend builds for instant dual-instance local network debugging, transitioning to IL2CPP for final production deployment.</li>
      </ul>
    </td>
  </tr>
</table>


<br />

<!-- SECTION 04: ARCHITECTURE & WORKFLOW DEEP DIVES -->
<h3>06 // TECHNICAL SPECIFICATIONS & WORKFLOWS</h3>

<details open>
<summary><b>SPEC 01 // MULTIPLAYER SYNC & RPC PIPELINE (Click to expand)</b></summary>
<br />

```text
[ Client Input ] ──> [ Local Prediction / Immediate Feedback ]
       
[ PurrNet/Networking RPC / State Sync ] ──> [ Host / Server Validation ]
       │
       ├──> [ Authoritative State ] ──> Broadcast to Peers (Transforms, Inventory, Health)
       └──> [ Cosmetic Impact ]     ──> Executed Locally (Decals, Particle Systems, Audio)
```
</details>

<details>
<summary><b>SPEC 02 // CROSS-PLATFORM BUILD & DEPLOYMENT TARGETS (Click to expand)</b></summary>
<br />
<table width="100%">
  <tr>
    <th align="left">Platform</th>
    <th align="left">Backend / API</th>
    <th align="left">Optimization Focus</th>
  </tr>
  <tr>
    <td><b>Windows (PC)</b></td>
    <td>Mono (Dev) / IL2CPP (Prod), DirectX 11/12</td>
    <td>Fast iteration compilation during netcode testing; high-refresh-rate frame pacing and shader fidelity.</td>
  </tr>
  <tr>
    <td><b>Android (Mobile)</b></td>
    <td>IL2CPP, ARM64, OpenGL ES / Vulkan</td>
    <td>Draw call batching, baked lightmaps, touch UI responsiveness, and thermal/memory footprint reduction.</td>
  </tr>
  <tr>
    <td><b>WebGL (Browser)</b></td>
    <td>WASM, Brotli Compression</td>
    <td>Asset bundle size minimization, asynchronous loading, and stripped engine modules for fast web startup.</td>
  </tr>
</table>
</details>

<br />

<!-- FOOTER -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=a259ff&height=2" width="100%" />
  <br />
  <p>
    <b>AVAILABLE FOR COLLABORATION ON MULTIPLAYER PROJECTS, SYSTEMS ENGINEERING & GAME DEVELOPMENT</b>
  </p>
  <sub>// Thank you for reading!  //  </sub>
</div>
