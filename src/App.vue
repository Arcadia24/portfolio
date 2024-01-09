<template>
  <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>

  <!-- <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div> -->

  <header class="header">
    <a href="#" class="logo">Nathan. <span class="animate" style="--i:1;"></span></a>

    <i class='bx bx-menu' id="menu-icon"></i>

    <nav class="navbar">
      <a href="#home" @click.prevent="scrollToSection('home')" :class="{ 'active': activeSection === 'home' }">home</a>
      <a href="#about" @click.prevent="scrollToSection('about')" :class="{ 'active': activeSection === 'about' }">about</a>
      <a href="#education" @click.prevent="scrollToSection('education')" :class="{ 'active': activeSection === 'education' }">education</a>
      <a href="#projects" @click.prevent="scrollToSection('projects')" :class="{ 'active': activeSection === 'projects' }">projects</a>
      <a href="#skills" @click.prevent="scrollToSection('skills')" :class="{ 'active': activeSection === 'skills' }">skills</a>
      <!-- <a href="#contact" @click.prevent="scrollToSection('contact')" :class="{ 'active': activeSection === 'contact' }">contact</a> -->

      <span class="active-navbar"></span>
      <span class="animate" style="--i:2;"></span>
    </nav>
  </header>

  <section class="home" id="home" :class="{ 'show-animate': activeSection === 'home' }" ref="sections">
    <div class="home-content">
      <h1>Hi, I'm <span>Nathan Vidal</span><span class="animate" style="--i:2;"></span></h1>
      <div class="text-animate">
        <h3>Creative Technololist Student</h3>
        <span class="animate" style="--i:3;"></span>
      </div>
      <p>I'm currently diving into the world of creative technology. 
        I'm captivated by the potential of artificial intelligence, the nature, and the stunning world of art. 
        My days are filled with experimenting and finding new ways to combine these diverse elements. It's all about seeing how AI can enhance the beauty of nature and the creativity of art. 
        I'm on a quest to discover the intersections where technology meets the organic and where digital innovation can amplify artistic creativity.
      <span class="animate" style="--i:4;"></span>
      </p>
      <div class="btn-box">
        <!-- <a href="#" class="btn">Hire Me</a>
        <a href="#contact" class="btn">Let's Talk</a>
        <span class="animate" style="--i:5;"></span> -->
      </div>
    </div>

    <div class="home-sci">
      <a href="https://github.com/Arcadia24" ><i class='bx bxl-github'></i></a>
      <a href="https://www.linkedin.com/in/nathan-vidal/" ><i class='bx bxl-linkedin'></i></a>
      <span class="animate" style="--i:6;"></span>
    </div>

     <div class="home-canvas">
      <canvas id="canvas"></canvas>
     </div>



  </section>

  <section class="about" id="about" :class="{ 'show-animate': activeSection === 'about' }" ref="sections" >
    <h2 class="heading">About <span>Me</span><span class="animate scroll" style="--i:2;"></span></h2>
    <div class="about-img">
      <img src="./assets/VIDALNathan-3.jpg" width="400" length="400">
      <span class="circle-spin"></span>
      <span class="animate scroll" style="--i:2;"></span>
    </div>

    <div class="about-content">
      <h3>Creative Technololist Student<span class="animate scroll" style="--i:2;"></span></h3>
      <p>
        I'm a student of creative technology, deeply fascinated by artificial intelligence, 
        the wonders of nature, and the beauty of art. My work revolves around blending these elements together. 
        I'm all about figuring out how AI can help us get closer to nature and art.
        <span class="animate scroll" style="--i:2;"></span>
      </p>
    </div>

    <div class="btn-box btns">
      <a href="https://dvic.devinci.fr/member/nathan-vidal" class="btn">Read More</a>
      <span class="animate scroll" style="--i:2;"></span>
    </div>
  </section>

  <section class="education" id="education" :class="{ 'show-animate': activeSection === 'education' }" ref="sections">
    <h2 class="heading">My <span>Journey</span><span class="animate scroll" style="--i:1;"></span></h2>

    <div class="education-row">
      <div class="education-column">
        <h3 class="title">Education<span class="animate scroll" style="--i:2;"></span></h3>

        <div class="education-box">
          <div class="education-content">
            <div class="content">
              <div class="year"><i class="bx bxs-calendar"></i> 2022 - 2024</div>
              <h3>MS Creative Technology at Institute for Future Techonologies</h3>
              <p>I pursued a Master of Science in Creative Technology at the De Vinci Innovation Center, 
                focusing on the intersection of technology, innovation, and design.</p>
            </div>
          </div>

          <div class="education-content">
            <div class="content">
              <div class="year"><i class="bx bxs-calendar"></i> 2021 - 2024</div>
              <h3>Master’s in Engineering at Leonard De Vinci Engineer School</h3>
              <p>I completed a Master's degree in Data Science at École Supérieure d'Ingénieurs Léonard de Vinci (ESILV) where I honed my skills in analytics, machine learning, and big data technologies.</p>
            </div>
          </div>

          <div class="education-content">
            <div class="content">
              <div class="year"><i class="bx bxs-calendar"></i> 2020 - 2021</div>
              <h3>Post-graduate Preparatory Class at Saint-Cyr L’ ́ecole Militar High School</h3>
              <p>Two years of rigorous coursework in preparation for the engineering school entrance exam in France.</p>
            </div>
          </div>
          <span class="animate scroll" style="--i:3;"></span>
        </div>
      </div>

      <div class="education-column">
        <h3 class="title">Experience<span class="animate scroll" style="--i:5;"></span></h3>

        <div class="education-box">
          <div class="education-content">
            <div class="content">
              <div class="year"><i class="bx bxs-calendar"></i> Apr 2023 - Aug 2023</div>
              <h3>Data Scientist intern in Danish Crown</h3>
              <p> Forecast cattle exportation over 15 months for beef business unit.
                  Creation of a dataset of hides tag of more than 3000 images and videos, labeling it and train an image
                  segmentation model to recognize the tags for a subsidiary</p>
            </div>
          </div>

          <div class="education-content">
            <div class="content">
              <div class="year"><i class="bx bxs-calendar"></i> Oct 2021 - Jun 2022</div>
              <h3>Developer in junior enterprise</h3>
              <p>Developing a data scraping bot for requests for job proposals using python and google API. Deploying
                them on a web server using Docker.</p>
            </div>
          </div>

          <div class="education-content">
            <div class="content">
              <div class="year"><i class="bx bxs-calendar"></i> Jul 2020</div>
              <h3>Superior Military Preparation</h3>
              <p>2 weeks preparation in French land forces College to get graduate as a corporal in reserve.</p>
            </div>
          </div>
          <span class="animate scroll" style="--i:6;"></span>
        </div>
      </div>
    </div>
  </section>

  <section class="projects" id="projects" :class="{ 'show-animate': activeSection === 'projects' }" ref="sections">
    <h2 class="heading">My <span>Projects</span></h2>
    <div class="project-row">
      <div class="project-card">
        <a href="https://dvic.devinci.fr/projects/cui-cui" target="_blank">
        <img src="./assets/cuicui.png" alt="Project Image" />
        <h2>Cui-cui Project</h2>
        <p>Classifier of bird species by sound</p>
        </a>
      </div>
      <div class="project-card">
        <a href="https://dvic.devinci.fr/projects/food-computer" target="_blank">
        <img src="./assets/foodcomputerlogo.jpg" alt="Project Image" />
        <h2>Food Computer</h2>
        <p>Controlled Environments Agriculture</p>
        </a>
      </div>
    </div>
    <div class="project-row">
      <div class="project-card">
        <a href="https://dvic.devinci.fr/quickstarter/the-leather-page" target="_blank">
        <img src="./assets/TLP.png" alt="Project Image" />
        <h2>The Leather Page</h2>
        <p>QuickStarter project</p>
        </a>
      </div>
      <div class="project-card">
        <a href="https://dvic.devinci.fr/projects/gosai" target="_blank">
        <img src="./assets/gosaiLOGO.png" alt="Project Image" />
        <h2>GOSAI</h2>
        <p>General-purpose Operating System for Augmented Interfaces</p>
        </a>
      </div>
    </div>
    <div class="project-row">
      <div class="project-card">
        <a href="https://github.com/Arcadia24/calculator" target="_blank">
        <img src="./assets/MNIST.png" alt="Project Image" />
        <h2>Calculator</h2>
        <p>Hand-Written Calculator using Deep Learing on Expand-MNIST</p>
        </a>
      </div>
      <div class="project-card">
        <a href="https://github.com/Arcadia24/TTS-with-emotion-conversion" target="_blank">
        <img src="./assets/theatre2.png" alt="Project Image" />
        <h2>StageWhisper</h2>
        <p>Application on GOSAI Interface to show the use of audio interaction</p>
        </a>
      </div>
    </div>
  </section>
  <section class="skills" id="skills" :class="{ 'show-animate': activeSection === 'skills' }" ref="sections">
    <h2 class="heading">My <span>Skills</span><span class="animate scroll" style="--i:1;"></span></h2>

    <div class="skills-row">
      <div class="skills-column">
        <h3 class="title">Coding Skills<span class="animate scroll" style="--i:2;"></span></h3>

        <div class="skills-box">
          <div class="skills-content">
            <div class="progress">
              <h3>Python <span>90%</span></h3>
              <div class="bar"><span></span></div>
            </div>

            <div class="progress">
              <h3>HTML/CSS/JS <span>80%</span></h3>
              <div class="bar"><span></span></div>
            </div>

            <div class="progress">
              <h3>C# <span>65%</span></h3>
              <div class="bar"><span></span></div>
            </div>

            <div class="progress">
              <h3>C <span>50%</span></h3>
              <div class="bar"><span></span></div>
            </div>
          </div>
          <span class="animate scroll" style="--i:3;"></span>
        </div>
      </div>

      <div class="skills-column">
        <h3 class="title">Professional Skills<span class="animate scroll" style="--i:5;"></span></h3>

        <div class="skills-box">
          <div class="skills-content">
            <div class="progress">
              <h3>Deep Learning <span>80%</span></h3>
              <div class="bar"><span></span></div>
            </div>

            <div class="progress">
              <h3>Machine Learning <span>70%</span></h3>
              <div class="bar"><span></span></div>
            </div>

            <div class="progress">
              <h3>Web Dev <span>50%</span></h3>
              <div class="bar"><span></span></div>
            </div>

            <div class="progress">
              <h3>CI/CD <span>60%</span></h3>
              <div class="bar"><span></span></div>
            </div>
          </div>
          <span class="animate scroll" style="--i:6;"></span>
        </div>
      </div>
    </div>

  </section>

  <footer class="footer">
    <div class="foote-text">
      <p>Copyright &copy; 2023 by Nathan Vidal | All Rights Reserved.</p>
    </div>

    <div class="footer-iconTop">
      <a href="#"><i class='bx bx-up-arrow-alt'></i></a>
    </div>
  </footer>

</template>

<script>
import * as THREE from 'three';
import { OrbitControls } from 'three/examples/jsm/controls/OrbitControls.js';
import { EffectComposer } from 'three/examples/jsm/postprocessing/EffectComposer.js';
import { RenderPass } from 'three/examples/jsm/postprocessing/RenderPass.js';
import { UnrealBloomPass } from 'three/examples/jsm/postprocessing/UnrealBloomPass.js';
import { OutputPass } from 'three/examples/jsm/postprocessing/OutputPass.js';
export default {

  data() {
    return {
      isMenuOpen: false,
      isSticky: false,
      sections: [
        { id: 'home', title: 'home' },
        { id: 'about', title: 'about' },
        { id: 'education', title: 'education' },
        { id: 'projects', title: 'projects' },
        { id: 'skills', title: 'skills' },
        // Add more sections as needed
      ],
      activeSection: null,
    };
  },
  methods: {
    visitProject(link) {
      window.open(link, "_blank");
    },
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
    scrollToSection(sectionId) {
      const targetSection = document.getElementById(sectionId);
      if (targetSection) {
        window.scrollTo({
          top: targetSection.offsetTop,
          behavior: 'smooth',
        });
      }
      this.isMenuOpen = false;
    },
    handleScroll() {
      const top = window.scrollY;
      const sections = this.sections.map((section) => section.id);

      for (let i = sections.length - 1; i >= 0; i--) {
        const sectionId = sections[i];
        const sectionElement = document.getElementById(sectionId);
        if (sectionElement) {
          const offset = sectionElement.offsetTop - 100;
          const height = sectionElement.offsetHeight;

          if (top >= offset && top < offset + height) {
            this.activeSection = sectionId;
            return;
          }
        }
      }
      this.activeSection = null;
      this.isSticky = top > 100;
    },
    initThreeJS(){

      const params = {
          red: 1.0,
          green: 1.0,
          blue: 1.0,
          treshold: 0.7,
          strenght: 0.4,
          radius: 0.4
      };

      // Create a scene
      const scene = new THREE.Scene();

      // Create a camera
      const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
      camera.position.set(0, 0, 10);

      // Import the canvas element
      const canvas = document.getElementById('canvas');

      // Create a WebGLRenderer and set its width and height
      const renderer = new THREE.WebGLRenderer({
          canvas: canvas,
          // Antialiasing is used to smooth the edges of what is rendered
          antialias: true,
          // Activate the support of transparency
          alpha: true
      });

      renderer.setSize( window.innerWidth, window.innerHeight );
      renderer.setPixelRatio( window.devicePixelRatio );
      renderer.outputColorSpace = THREE.SRGBColorSpace;

      const composer = new EffectComposer( renderer );
      const renderPass = new RenderPass( scene, camera );

      const bloomPass = new UnrealBloomPass( new THREE.Vector2( window.innerWidth, window.innerHeight ));
      bloomPass.threshold = params.treshold;
      bloomPass.strength = params.strenght;
      bloomPass.radius = params.radius;
      composer.addPass( renderPass );
      composer.addPass( bloomPass );

      const outputPass = new OutputPass();
      composer.addPass( outputPass );

      // Create the controls
      const controls = new OrbitControls(camera, canvas);

      // Handle the window resize event
      window.addEventListener('resize', () => {
          // Update the camera
          camera.aspect =  window.innerWidth / window.innerHeight;
          camera.updateProjectionMatrix();

          // Update the renderer
          renderer.setSize(window.innerWidth, window.innerHeight);
          renderer.setPixelRatio(window.devicePixelRatio);
          composer.setSize(window.innerWidth, window.innerHeight);
      });

      // Create the uniforms

      const uniforms = {
          u_resolution: { type: 'v2', value: new THREE.Vector2(window.innerWidth, window.innerHeight) },
          u_time: { type: 'f', value: 0.0 },
          u_frequency: { type: 'f', value: 0.0 },
      };


      // Create the sphere
      const geometry = new THREE.IcosahedronGeometry(4, 30);
      const material = new THREE.ShaderMaterial({
          uniforms,
          vertexShader: `
            uniform float u_time;
            uniform float u_frequency;
            vec3 mod289(vec3 x)
            {
            return x - floor(x * (1.0 / 289.0)) * 289.0;
            }

            vec4 mod289(vec4 x)
            {
            return x - floor(x * (1.0 / 289.0)) * 289.0;
            }

            vec4 permute(vec4 x)
            {
            return mod289(((x*34.0)+10.0)*x);
            }

            vec4 taylorInvSqrt(vec4 r)
            {
            return 1.79284291400159 - 0.85373472095314 * r;
            }

            vec3 fade(vec3 t) {
            return t*t*t*(t*(t*6.0-15.0)+10.0);
            }
            float pnoise(vec3 P, vec3 rep)
            {
            vec3 Pi0 = mod(floor(P), rep); // Integer part, modulo period
            vec3 Pi1 = mod(Pi0 + vec3(1.0), rep); // Integer part + 1, mod period
            Pi0 = mod289(Pi0);
            Pi1 = mod289(Pi1);
            vec3 Pf0 = fract(P); // Fractional part for interpolation
            vec3 Pf1 = Pf0 - vec3(1.0); // Fractional part - 1.0
            vec4 ix = vec4(Pi0.x, Pi1.x, Pi0.x, Pi1.x);
            vec4 iy = vec4(Pi0.yy, Pi1.yy);
            vec4 iz0 = Pi0.zzzz;
            vec4 iz1 = Pi1.zzzz;

            vec4 ixy = permute(permute(ix) + iy);
            vec4 ixy0 = permute(ixy + iz0);
            vec4 ixy1 = permute(ixy + iz1);

            vec4 gx0 = ixy0 * (1.0 / 7.0);
            vec4 gy0 = fract(floor(gx0) * (1.0 / 7.0)) - 0.5;
            gx0 = fract(gx0);
            vec4 gz0 = vec4(0.5) - abs(gx0) - abs(gy0);
            vec4 sz0 = step(gz0, vec4(0.0));
            gx0 -= sz0 * (step(0.0, gx0) - 0.5);
            gy0 -= sz0 * (step(0.0, gy0) - 0.5);

            vec4 gx1 = ixy1 * (1.0 / 7.0);
            vec4 gy1 = fract(floor(gx1) * (1.0 / 7.0)) - 0.5;
            gx1 = fract(gx1);
            vec4 gz1 = vec4(0.5) - abs(gx1) - abs(gy1);
            vec4 sz1 = step(gz1, vec4(0.0));
            gx1 -= sz1 * (step(0.0, gx1) - 0.5);
            gy1 -= sz1 * (step(0.0, gy1) - 0.5);

            vec3 g000 = vec3(gx0.x,gy0.x,gz0.x);
            vec3 g100 = vec3(gx0.y,gy0.y,gz0.y);
            vec3 g010 = vec3(gx0.z,gy0.z,gz0.z);
            vec3 g110 = vec3(gx0.w,gy0.w,gz0.w);
            vec3 g001 = vec3(gx1.x,gy1.x,gz1.x);
            vec3 g101 = vec3(gx1.y,gy1.y,gz1.y);
            vec3 g011 = vec3(gx1.z,gy1.z,gz1.z);
            vec3 g111 = vec3(gx1.w,gy1.w,gz1.w);

            vec4 norm0 = taylorInvSqrt(vec4(dot(g000, g000), dot(g010, g010), dot(g100, g100), dot(g110, g110)));
            g000 *= norm0.x;
            g010 *= norm0.y;
            g100 *= norm0.z;
            g110 *= norm0.w;
            vec4 norm1 = taylorInvSqrt(vec4(dot(g001, g001), dot(g011, g011), dot(g101, g101), dot(g111, g111)));
            g001 *= norm1.x;
            g011 *= norm1.y;
            g101 *= norm1.z;
            g111 *= norm1.w;

            float n000 = dot(g000, Pf0);
            float n100 = dot(g100, vec3(Pf1.x, Pf0.yz));
            float n010 = dot(g010, vec3(Pf0.x, Pf1.y, Pf0.z));
            float n110 = dot(g110, vec3(Pf1.xy, Pf0.z));
            float n001 = dot(g001, vec3(Pf0.xy, Pf1.z));
            float n101 = dot(g101, vec3(Pf1.x, Pf0.y, Pf1.z));
            float n011 = dot(g011, vec3(Pf0.x, Pf1.yz));
            float n111 = dot(g111, Pf1);

            vec3 fade_xyz = fade(Pf0);
            vec4 n_z = mix(vec4(n000, n100, n010, n110), vec4(n001, n101, n011, n111), fade_xyz.z);
            vec2 n_yz = mix(n_z.xy, n_z.zw, fade_xyz.y);
            float n_xyz = mix(n_yz.x, n_yz.y, fade_xyz.x); 
            return 2.2 * n_xyz;
            }

            void main() {
                float noise = 5.0 * pnoise(position + u_time, vec3(10.0));
                float displacement = (u_frequency / 20.0) * (noise / 30.0);
                vec3 newPosition = position + normal * displacement;
                gl_Position = projectionMatrix * modelViewMatrix * vec4( newPosition, 1.0 );
            }
          `,
          fragmentShader: `
            uniform float u_resolution;
            void main() {
            
                vec2 st = gl_FragCoord.xy/u_resolution;

                gl_FragColor = vec4(vec3(1.0,1.0, 1.0), 1.0);
            }
          `
      });
      const mesh = new THREE.Mesh(geometry, material);
      scene.add(mesh);
      mesh.material.wireframe = true;
      mesh.position.x += 5;

      const listener = new THREE.AudioListener();
      camera.add(listener);

      const sound = new THREE.Audio(listener);
      const analyser = new THREE.AudioAnalyser(sound, 32);

      const handleSuccess = function (stream) {
          const audioContext = listener.context; // Use the listener's audio context
          const mediaStreamSource = audioContext.createMediaStreamSource(stream);
          sound.setNodeSource(mediaStreamSource);
      };

      navigator.mediaDevices
          .getUserMedia({audio: true, video: false})
          .then(handleSuccess)
          .catch(e => console.error(e));

      // Function to resume audio context after user interaction
      function resumeAudioContext() {
          if (listener.context.state === "suspended") {
              listener.context.resume().then(() => {
                  console.log("AudioContext resumed!");
              }).catch(e => console.error(e));
          }
          // Remove the event listener after it has been called
          document.removeEventListener('click', resumeAudioContext);
      }

      // Add the event listener for user interaction
      document.addEventListener('click', resumeAudioContext);


      const clock = new THREE.Clock();

      // Create the animation loop
      const animate = () => {
          // Update the time uniform
          uniforms.u_time.value = clock.getElapsedTime();
          uniforms.u_frequency.value = analyser.getAverageFrequency();
          // Call animate recursively
          requestAnimationFrame(animate);

          // Update the controls
          controls.update();

          // Update the composer
          composer.render();

          // // Render the scene
          // renderer.render(scene, camera);
      }

      // Call animate for the first time
      animate();
    }
  },
  mounted() {
    this.initThreeJS();
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeUnmount() {
    window.removeEventListener('scroll', this.handleScroll);
  },
};

</script>

<style>

@import url('https://fonts.googleapis.com/css?family=Poppins:400,500,600,700&display=swap');

* {
  font-family: Poppins, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  border: none;
  outline: none;
  scroll-behavior: smooth;
}

:root{
  --bg-color: #081b29;
  --second-bg-color: #112e42;
  --text-color: #ededed;
  --main-color: #00abf0;
}

html {
  font-size: 62.5%;
  overflow-x: hidden;
}

body {
  background-color: var(--bg-color);
  color: var(--text-color);
}
canvas {
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}
a:visited {
  color: var(--text-color); /* Replace with your desired color */
}

.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 2rem 9%;
  background-color: var(--bg-color);
  display: flex;
  justify-content: space-between;
  align-items: safe;
  z-index: 100;
  transition: .3s;
}

.header.sticky {
  background: var(--bg-color);
}

.logo{
  color: var(--text-color);
  font-size: 2.5rem;
  font-weight: 600;
  letter-spacing: 0.2rem;
  position: relative;
}

.navbar {
  position: relative;
}

.navbar a {
  font-size: 1.7rem;
  color: var(--text-color);
  font-weight: 500;
  margin-left: 3.5rem;
  transition: .3s;
}

.navbar a:hover,
.navbar a.active{
  color: var(--main-color);
}

#menu-icon{
  font-size: 3.6rem;
  color: var(--text-color);
  cursor: pointer;
  display: none;
}

section{
  padding: 10rem 9% 2rem;
  min-height: 100vh;
}

.home{
  display: flex;
  align-items: center;
  padding: 0 9%;
  /* background: url('../assets/fond2.jpg') no-repeat;
  background-size: cover;
  background-position: 350px; */
}

.home-content{
  max-width: 60rem;
  z-index: 99;
}

.home-content h1{
  position: relative;
  display: inline-block;
  font-size: 5.6rem;
  font-weight: 700;
  line-height: 1.3;
}

.home-content h1 span {
  color: var(--text-color);
}

.home-content .text-animate{
  position: relative;
  width: 50rem; /* 32.8rem si 3 icon */
}

.home-content .text-animate h3{
  font-size: 3.2rem;
  font-weight: 700;
  color: transparent;
  -webkit-text-stroke: .7px var(--main-color);
  background-image: linear-gradient(var(--main-color), var(--main-color));
  background-repeat: no-repeat;
  -webkit-background-clip: text;
  background-position: -50rem 0;
  animation: homeBgText 6s linear infinite;
  animation-delay: 2s;
}

.home-content .text-animate h3::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 100%;
  border-right: 2px solid var(--main-color);
  z-index: -1;
  animation: homeCursorText 6s linear infinite;
  animation-delay: 2s;
}

.home-content p{
  position: relative;
  font-size: 1.6rem;
  margin: 2rem 0 4rem;
}

.btn-box{
  position: relative;
  display: flex;
  justify-content: space-between;
  width: 34.5rem;
  height: 5rem;
}

.btn-box .btn{
  position: relative;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  width: 15rem;
  height: 100%;
  background: var(--main-color);
  border: .2rem solid var(--main-color);
  border-radius: .8rem;
  font-size: 1.8rem;
  font-weight: 600;
  letter-spacing: .1rem;
  color: var(--bg-color);
  z-index: 1;
  overflow: hidden;
  transition: .5s;
}

.btn-box .btn:hover{
  color: var(--main-color);
}

.btn-box .btn:nth-child(2){
  background: transparent;
  color: var(--main-color);
}

.btn-box .btn:nth-child(2):hover{
  color: var(--bg-color);
}

.btn-box .btn:nth-child(2)::before{
  background: var(--main-color);
}

.btn-box .btn::before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 100%;
  background: var(--bg-color);
  z-index: -1;
  transition: all 0.6s ease;
}

.btn-box .btn:hover::before{
  width: 100%;
}

.home-sci {
  position: absolute;
  bottom: 4rem;
  width: 100px; /* 170px si 3 icon */
  display: flex;
  justify-content: space-between;
}

.home-sci a{
  position: relative;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  width: 40px;
  height: 40px;
  background: transparent;
  border: .2rem solid var(--main-color);
  border-radius: 50%;
  font-size: 20px;
  color: var(--main-color);
  z-index: 1;
  overflow: hidden;
  transition: .5s;
}

.home-sci a:hover{
  color: var(--bg-color);
}


.home-sci a::before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 100%;
  background: var(--main-color);
  z-index: -1;
  transition: all 0.6s ease;
}

.home-sci a:hover::before{
  width: 100%;
}

.about{
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 2rem;
  background: var(--second-bg-color);
  padding-bottom: 6rem;
}

.heading{
  position: relative;
  font-size: 5rem;
  margin-bottom: 3rem;
  text-align: center;
}

span{
  color: var(--main-color);
}

.about-img{
  position: relative;
  width: 40rem;
  height: 40rem;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.about-img img{
  border-radius: 50%;
  border: .2rem solid var(--main-color);
}

.about-img .circle-spin{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%) rotate(0);
  width: 100%;
  height: 100%;
  border-radius: 50%;
  border-top: .2rem solid var(--second-bg-color);
  border-bottom: .2rem solid var(--second-bg-color);
  border-right: .2rem solid var(--main-color);
  border-left: .2rem solid var(--main-color);
  animation: aboutSpinner 20s linear infinite;
}

.about-content{
  text-align: center;
}

.about-content h3{
  font-size: 2.6rem;
  position: relative;
  display: inline-block;
}

.about-content p{
  position: relative;
  font-size: 1.6rem;
  margin: 2rem 0 4rem;
}

.btn-box.btns{
  position: relative;
  display: inline-block;
  width: 15rem;
}

.btn-box.btns a::before{
  background: var(--second-bg-color);
}

.education{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  min-height: auto;
  padding-bottom: 5rem;
}

.education .education-row{
  display: flex;
  flex-wrap: wrap;
  gap: 5rem;
}

.education-row .education-column{
  flex: 1 1 40rem;
}

.education-column .title {
  position: relative;
  display: inline-block;
  font-size: 2.5rem;
  margin: 0 0 1.5rem 2rem;
}

.education-column .education-box{
  position: relative;
  border-left: .2rem solid var(--main-color);
}

.education-box .education-content{
  position: relative;
  padding: 2rem;
}

.education-box .education-content::before{
  content: '';
  position: absolute;
  top: 0;
  left: -1.1rem;
  width: 2rem;
  height: 2rem;
  background: var(--main-color);
  border-radius: 50%;
}

.education-content .content{
  position: relative;
  padding-left: 1.5rem;
  border: .2rem solid var(--main-color);
  border-radius: .6rem;
  margin-bottom: 2rem;
  overflow: hidden;
}

.education-content .content::before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 100%;
  background: var(--second-bg-color);
  z-index: -1;
  transition: .5s;
}

.education-content .content:hover::before{
  width: 100%;
}

.education-content .content .year{
  font-size: 1.5rem;
  color: var(--main-color);
  padding-bottom: 1rem;
}

.education-content .content .year i {
  padding-right: .5rem;
}

.education-content .content h3 {
  font-size: 2rem;
}

.education-content .content p {
  font-size: 1.6rem;
  margin-bottom: 0.5rem;
}

.skills {
  min-height: auto;
  padding-bottom: 7rem;
}

.skills h2 {
  display: inline-block;
  left: 50%;
  transform: translateX(-50%);
}

.skills .skills-row{
  display: flex;
  flex-wrap: wrap;
  gap: 5rem;
}

.skills-row .skills-column{
  flex: 1 1 40rem;
}

.skills-column .title {
  position: relative;
  display: inline-block;
  font-size: 2.5rem;
  margin: 0 0 1.5rem;
}

.skills-column .skills-box{
  position: relative;
}

.skills-box .skills-content{
  position: relative;
  border: .2rem solid var(--main-color);
  border-radius: .6rem;
  padding: .5rem 1.5rem;
  z-index: 1;
  overflow: hidden;
}

.skills-box .skills-content::before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 100%;
  background: var(--bg-color);
  z-index: -1;
  transition: .8s;
}

.skills-box .skills-content:hover::before{
  width: 100%;
}

.skills-content .progress{
  padding: 1rem 0;
}

.skills-content .progress h3{
  font-size: 1.7rem;
  display: flex;
  justify-content: space-between;
}

.skills-content .progress h3 span {
  color: var(--text-color);
}

.skills-content .progress .bar {
  height: 2.5rem;
  border-radius: .6rem;
  border: .2rem solid var(--main-color);
  padding: .5rem;
  margin: 1rem 0;
}

.skills-content .progress .bar span {
  display: block;
  height: 100%;
  background: var(--main-color);
  border-radius: .3rem;
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(1) .bar span {
  width: 90%;
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(2) .bar span {
  width: 80%;
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(3) .bar span {
  width: 65%;
}

.skills-column:nth-child(1) .skills-content .progress:nth-child(4) .bar span {
  width: 50%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(1) .bar span {
  width: 80%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(2) .bar span {
  width: 70%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(3) .bar span {
  width: 50%;
}

.skills-column:nth-child(2) .skills-content .progress:nth-child(4) .bar span {
  width: 60%;
}


.project-row {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
}

.project-card {
  text-align: center;
  width: calc(50% - 10px); /* Two cards per row with some spacing */
  margin-bottom: 20px;
  padding: 1rem 5rem; /* Increased padding for larger cards */
  border: .2rem solid var(--main-color);
  border-radius: 2rem; /* Larger border radius for rounded corners */
  background-color: var(--second-bg-color);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  cursor: pointer;
  transition: transform 0.2s;
}

.project-card:hover {
  transform: scale(1.05);
}

.project-card img {
  width: 300px;
  height: 300px;
  margin-bottom: 15px; /* Slightly increased margin for image */
}

.project-card h2 {
  font-size: 24px; /* Larger font size for the project name */
  margin: 0 10;
}

.project-card p {
  font-size: 18px; /* Larger font size for the project description */
  margin: 10px 0;
}

.contact {
  min-height: auto;
  padding-bottom: 7rem;
  background: var(--second-bg-color);
}

.contact h2 {
  display: inline-block;
  left: 50%;
  transform: translateX(-50%);
}

.contact form{
  max-width: 70rem;
  margin: 0 auto;
  text-align: center;
}

.contact form .input-box {
  position: relative;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.contact form .input-box .input-field {
  position: relative;
  width: 49%;
  margin: .8rem 0;
}

.contact form .input-box .input-field input,
.contact form .textarea-field textarea{
  width: 100%;
  height: 100%;
  padding: 1.5rem;
  font-size: 1.6rem;
  color: var(--text-color);
  background: transparent;
  border-radius: .6rem;
  border: .2rem solid var(--main-color);
}

.contact form .input-box .input-field input::placeholder,
.contact form .textarea-field textarea::placeholder {
  color: var(--text-color);
}

.contact form .focus{
  position: absolute;
  width: 0;
  height: 100%;
  top: 0;
  left: 0;
  background: var(--bg-color);
  border-radius: .6rem;
  z-index: -1;
  transition: .5s;
}

.contact form .input-box .input-field input:focus ~ .focus,
.contact form .input-box .input-field input:valid ~ .focus
.contact form .textarea-field textarea:focus ~ .focus,
.contact form .textarea-field textarea:valid ~ .focus {
  width: 100%;
}

.contact form .textarea-field {
  position: relative;
  margin: .8rem 0 2.7rem;
  display: flex;
}

.contact form .textarea-field textarea {
  resize: none;
}

.contact form .btn-box.btns .btn {
  cursor: pointer;
}

.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  padding: 2rem 9%;
  background: var(--bg-color);
}

.footer-text p {
  font-size: 1.6rem;
}

.footer-iconTop a {
  position: relative;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  padding: .8rem;
  background: var(--bg-color);
  border: .2rem solid var(--main-color);
  border-radius: .6rem;
  z-index: 1;
  overflow: hidden;
}

.footer-iconTop a::before{
  content: '';
  position: absolute;
  top:0;
  left: 0;
  width: 0;
  height: 100%;
  background: var(--second-bg-color);
  z-index: -1;
  transition: .5s;
}

.footer-iconTop a:hover::before{
  width: 100%;
}

.footer-iconTop a i {
  font-size: 2.4rem;
  color: var(--main-color);
}

.footer-iconTop a:hover i {
  color: var(--main-color);
}

/* ANIMATION RELOAD AND SCROLL */
/*.animate {
  position: absolute;
  top: 0;
  right: 0;
  width: 100%;
  height: 100%;
  background: var(--bg-color);
  z-index: 98;
}

.animate.home-img {
  width: 50%;
}

.logo .animate,
.navbar .animate,
.home.show-animate .animate {
  animation: showRight 1s ease forwards;
  animation-delay: calc(.1s * var(--i));
}

.animate.scroll {
  transition: 1s ease;
  transition-delay: calc(.1s * var(--i));
  animation: none;
}


.education .education-box .animate.scroll {
  width: 105%;

}

.about.show-animate .animate.scroll,
.education.show-animate .animate.scroll,
.skills.show-animate .animate.scroll,
.contact.show-animate .animate.scroll
.projects.show-animate .animate.scroll{
  animation-delay: calc(.1s * var(--i));
  width: 0;
}*/

section:nth-child(even) /*.animate.scroll,
.footer .animate.scroll*/ {
  background: var(--second-bg-color);
}

/* BREAKPOINTS */
@keyframes homeBgText {
  0%, 10%, 100%{
    background-position: -50rem 0;
  }
  65%, 85%{
    background-position: 0 0;
  }

}

@keyframes homeCursorText {
  0%, 10%, 100%{
    width: 0;
  }
  65%, 78%, 85%{
    width: 100%;
    opacity: 1;
  }
  75%, 81%{
    opacity: 0;
  }

}

@keyframes aboutSpinner {
  0%{
    transform: translate(-50%, -50%) rotate(0);
  }
  100%{
    transform: translate(-50%, -50%) rotate(360deg);
  }
}

@keyframes showRight {
  100%{
    width: 0;
  }
}

/* media queries */

@media (max-width: 1200px) {
  html{
    font-size: 55%;
  }
}

@media (max-width: 991px) {
  html{
    font-size: 2rem 4%;
  }

  section {
    padding: 10rem 4% 2rem;
  }

  .home {
    padding: 0 4%;
  }

  .footer {
    padding: 2rem 4%;
  }
}

@media (max-width: 768px) {
  .header {
    background: var(--bg-color);
  }

  #menu-icon {
    display: block;
  }

  .navbar {
    position: absolute;
    top: 100%;
    left: 0;
    width: 100%;
    padding: 1rem 4%;
    background: var(--bg-color);
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0, 0.2);
  }

  .navbar a {
    display: block;
    font-size: 2rem;
    margin: 3rem 0;
  }
  .navbar.active{
  left: 0;
  transition-delay: 0s ;
  }

  .navbar .active-navbar {
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: var(--bg-color);
    border-top: .1rem solid rgba(0, 0, 0, 0.2);
    z-index: -1;
  }

  .navbar.active .active-navbar {
    transition-delay: .25s;
    left: 0;
  }

  .navbar a{
    font-size: 1.7rem;
    font-weight: 500;
    margin-left: 3.5rem;
    transition: all 0.3s ease;
    color: var(--text-color);
    transition: translateX(-20rem);
  }

  .navbar.active a{
    transition-delay: .25s;
    transition: translateX(0);
  }

.home-imgHover {
  pointer-events: none;
  background: var(--bg-color);
  opacity: .6;
}

}


</style>