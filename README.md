
<html>
<head>
  <title>Visor 3D</title>
  <style>
    #canvas {
      width: 100%;
      height: 100%;
      overflow: hidden;
    }
  </style>
</head>
<body>
<div id="header" align="center">
   <img src="https://gifdb.com/images/file/spooky-month-creepy-ghostemane-black-and-white-qvk7qe2jg709qjq2.gif" alt="Profile GIF" width="350">
   <h3>Hi, I'm Moises, a software engineer.<h3/>
   <p>
    <a href="https://instagram.com/moises_saucedo_ambicho?igshid=MzRlODBiNWFlZA==" target="_blank">
      <img src="https://i.ibb.co/p0pfgGv/instagram.png" width="20"/>
    </a>
     <a href="https://www.linkedin.com/in/moises-saucedo-ambicho-813316174" target="_blank">
      <img src="https://i.ibb.co/XVp5j8P/linkedin.png" width="20" />
    </a>
     <a href="https://www.reddit.com/user/moises_saucedoxd" target="_blank">
     <img src="https://i.ibb.co/cL1WZKP/reddit.png" width="20">
     </a>
  </p>
</div>

### <img src="https://i.ibb.co/MNNckFs/coffee-shop-unscreen.gif" width="40"> development skills
<hr/>   
  <p id="badges" align="center">
  <a href="https://skillicons.dev" target="_blank">
    <img src="https://skillicons.dev/icons?i=cs,php,js,html,css,sass,mysql,dotnet,laravel,react,postman,git" />
  </a>
</p>
   
### <img src="https://raw.githubusercontent.com/innng/innng/master/assets/kyubey.gif" width="60"/> Soft Skills
   <hr/>
   <ul>
      <li>Resilience</li>
      <li>teamwork</li>
      <li>Analytical and problem solving capacity</li>
      <li>Adaptability</li>
      <li>Desire to learn and be at the forefron</li>
   </ul>     
   
###  My Stats
 <hr/>
   <div align="center">
 <picture>
  <source
    srcset="https://github-readme-stats.vercel.app/api?username=MOISES1003&show_icons=true&theme=dark"/>
  <img src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true" />
</picture>  
 <picture>
  <source
    srcset="https://streak-stats.demolab.com?user=MOISES1003&hide_border=FALSO&border_radius=4.2&card_width=350&theme=dark"/>
  <img src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true" />
</picture>  
    <div/>
<picture>
  <source srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=MOISES1003&layout=compact&theme=dark"/>
  <img src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true" />
</picture>
 <div/>     

<div id="canvas"></div>
  <script src="https://cdn.jsdelivr.net/npm/three@0.134.0/build/three.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/three@0.134.0/examples/js/loaders/GLTFLoader.js"></script>
  <script>
    // Código de inicialización de Three.js y carga del modelo 3D
    const canvas = document.getElementById('canvas');
    const renderer = new THREE.WebGLRenderer();
    renderer.setSize(window.innerWidth, window.innerHeight);
    canvas.appendChild(renderer.domElement);

    const scene = new THREE.Scene();
    const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
    camera.position.z = 5;

    const loader = new THREE.GLTFLoader();
    loader.load(
      'img/MOISES1003-2022.gltf',
      function (gltf) {
        scene.add(gltf.scene);
      },
      undefined,
      function (error) {
        console.error(error);
      }
    );

    function animate() {
      requestAnimationFrame(animate);
      renderer.render(scene, camera);
    }

    animate();
  </script>   
</body>
</html>
 
