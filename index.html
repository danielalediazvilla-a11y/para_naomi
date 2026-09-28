import os
import webbrowser

# El código HTML y 3D interactivo de Naomi
codigo_html = """
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Universo Kraft: Naomi ✨</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
            background-color: #200814;
            font-family: 'Courier New', Courier, monospace;
            user-select: none;
        }
        .interfaz-mensajes {
            position: absolute;
            top: 25px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(48, 16, 32, 0.85);
            border: 4px solid #ff85a2;
            padding: 20px;
            border-radius: 4px;
            text-align: center;
            box-shadow: 0 0 25px rgba(255, 105, 180, 0.4);
            z-index: 100;
            width: 380px;
            max-width: 90%;
        }
        h1 {
            margin: 0 0 10px 0;
            font-size: 1.6rem;
            color: #ffb3c6;
            text-shadow: 2px 2px #000;
        }
        p {
            margin: 0 0 15px 0;
            font-size: 0.95rem;
            color: #ffffff;
            line-height: 1.4;
            text-shadow: 1px 1px #000;
        }
        button {
            background-color: #55444b;
            border: 3px solid #221115;
            border-top-color: #ffa6c9;
            border-left-color: #ffa6c9;
            color: #fff0f5;
            padding: 10px 15px;
            font-size: 1rem;
            font-weight: bold;
            font-family: inherit;
            cursor: pointer;
            box-shadow: inset 0 -4px #221115;
            width: 100%;
        }
        button:hover {
            background-color: #ff85a2;
            color: #200814;
            border-color: #4a1222;
            border-top-color: #ffe3ec;
            border-left-color: #ffe3ec;
        }
        .caja-aliento {
            display: none;
            margin-top: 15px;
            text-align: left;
        }
        .frase {
            font-size: 1.05rem;
            font-weight: bold;
            color: #ffc2d1;
            text-shadow: 2px 2px #000;
            margin: 8px 0;
            padding-left: 15px;
            position: relative;
        }
        .frase::before {
            content: '✦';
            position: absolute;
            left: 0;
            color: #ff477e;
        }
        .indicador-camara {
            position: absolute;
            bottom: 15px;
            left: 50%;
            transform: translateX(-50%);
            color: #ffb3c6;
            font-size: 0.8rem;
            text-shadow: 1px 1px #000;
            pointer-events: none;
            z-index: 100;
        }
    </style>
    <script src="https://cloudflare.com"></script>
    <script src="https://jsdelivr.net"></script>
</head>
<body>

    <div class="interfaz-mensajes">
        <h1>Mundo de: <span style="color:#ff477e;">Naomi</span> 🔍</h1>
        <p>Un espacio infinito creado en bloques para recordarte lo valiosa e importante que eres.</p>
        <button onclick="activarExploracion()">¡Abrir Cofre de Aliento!</button>
        
        <div id="seccionAliento" class="caja-aliento">
            <div class="frase">¡Eres una persona increíble!</div>
            <div class="frase">Tu genialidad no tiene límites.</div>
            <div class="frase">Capaz de superar cualquier reto.</div>
            <div class="frase">¡Sigue brillando con tu propia luz!</div>
        </div>
    </div>

    <div class="indicador-camara">AMantén presionado el clic izquierdo y arrastra para mover la cámara en 3D</div>

    <script>
        const scene = new THREE.Scene();
        scene.background = new THREE.Color(0x200814);
        scene.fog = new THREE.FogExp2(0x200814, 0.02);

        const camera = new THREE.PerspectiveCamera(65, window.innerWidth / window.innerHeight, 0.1, 1000);
        camera.position.set(0, 5, 28);

        const renderer = new THREE.WebGLRenderer({ antialias: false });
        renderer.setSize(window.innerWidth, window.innerHeight);
        document.body.appendChild(renderer.domElement);

        const controls = new THREE.OrbitControls(camera, renderer.domElement);
        controls.enableDamping = true;
        controls.dampingFactor = 0.05;

        const lightAmbient = new THREE.AmbientLight(0xffd6ff, 0.6);
        scene.add(lightAmbient);

        const lightDir = new THREE.DirectionalLight(0xff85a2, 1.2);
        lightDir.position.set(10, 30, 15);
        scene.add(lightDir);

        const bloqueGeo = new THREE.BoxGeometry(1, 1, 1);
        
        // Estrellas
        const estrellasGeo = new THREE.BufferGeometry();
        const numEstrellas = 400;
        const posicionesEstrellas = new Float32Array(numEstrellas * 3);
        for(let i=0; i<numEstrellas*3; i+=3) {
            posicionesEstrellas[i] = (Math.random() - 0.5) * 80;
            posicionesEstrellas[i+1] = (Math.random() - 0.5) * 60 + 10;
            posicionesEstrellas[i+2] = (Math.random() - 0.5) * 80;
        }
        estrellasGeo.setAttribute('position', new THREE.BufferAttribute(posicionesEstrellas, 3));
        const estrellasMat = new THREE.PointsMaterial({ size: 0.35, color: 0xffb3c6 });
        const estrellasNube = new THREE.Points(estrellasGeo, estrellasMat);
        scene.add(estrellasNube);

        // Nombre NAOMI en bloques
        const nombreGrupo = new THREE.Group();
        const matLetras = new THREE.MeshLambertMaterial({ color: 0xff477e });

        const letrasData = {
            N: [[1,0,0,0,1],[1,1,0,0,1],[1,0,1,0,1],[1,0,0,1,1],[1,0,0,0,1]],
            A: [[0,1,1,1,0],[1,0,0,0,1],[1,1,1,1,1],[1,0,0,0,1],[1,0,0,0,1]],
            O: [[0,1,1,1,0],[1,0,0,0,1],[1,0,0,0,1],[1,0,0,0,1],[0,1,1,1,0]],
            M: [[1,0,0,0,1],[1,1,0,1,1],[1,0,1,0,1],[1,0,0,0,1],[1,0,0,0,1]],
            I: [[1,1,1,1,1],[0,0,1,0,0],[0,0,1,0,0],[0,0,1,0,0],[1,1,1,1,1]]
        };

        const ordenLetras = ['N','A','O','M','I'];
        let despliegueX = -16;

        ordenLetras.forEach(letra => {
            const matriz = letrasData[letra];
            const grupoLetra = new THREE.Group();
            for (let r = 0; r < matriz.length; r++) {
                for (let c = 0; c < matriz[r].length; c++) {
                    if (matriz[r][c] === 1) {
                        const bloqueCubo = new THREE.Mesh(bloqueGeo, matLetras);
                        bloqueCubo.position.set(c, matriz.length - r, 0);
                        grupoLetra.add(bloqueCubo);
                    }
                }
            }
            grupoLetra.position.x = despliegueX;
            nombreGrupo.add(grupoLetra);
            despliegueX += 6.5;
        });
        nombreGrupo.position.set(-2, 8, -5);
        scene.add(nombreGrupo);

        // Cofre
        const cofreGrupo = new THREE.Group();
        const baseCofre = new THREE.Mesh(bloqueGeo, new THREE.MeshLambertMaterial({ color: 0xffc2d1 }));
        baseCofre.scale.set(2.5, 2, 2.5);
        cofreGrupo.add(baseCofre);
        const cerradura = new THREE.Mesh(bloqueGeo, new THREE.MeshLambertMaterial({ color: 0xff477e }));
        cerradura.scale.set(0.4, 0.6, 0.3);
        cerradura.position.set(0, 0.2, 1.3);
        cofreGrupo.add(cerradura);
        cofreGrupo.position.set(0, -3, 5);
        scene.add(cofreGrupo);

        let reloj = 0;
        function animate() {
            requestAnimationFrame(animate);
            reloj += 0.02;
            nombreGrupo.position.y = 8 + Math.sin(reloj * 1.5) * 0.4;
            nombreGrupo.rotation.y = Math.sin(reloj * 0.4) * 0.08;
            cofreGrupo.rotation.y += 0.01;
            estrellasNube.rotation.y += 0.0005;
            controls.update();
            renderer.render(scene, camera);
        }
        animate();

        window.addEventListener('resize', () => {
            camera.aspect = window.innerWidth / window.innerHeight;
            camera.updateProjectionMatrix();
            renderer.setSize(window.innerWidth, window.innerHeight);
        });

        function activarExploracion() {
            document.getElementById('seccionAliento').style.display = 'block';
            camera.position.set(0, 10, 18);
            controls.target.set(0, 9, -5);
        }
    </script>
</body>
</html>
"""

# Crea un archivo web temporal e inmediato
nombre_archivo = "index.html"
with open(nombre_archivo, "w", encoding="utf-8") as f:
    f.write(codigo_html)

# Abre el archivo en el navegador predeterminado de Linux Mint
ruta_absoluta = os.path.abspath(nombre_archivo)
webbrowser.open("file://" + ruta_absoluta)
print("¡Abriendo el universo de Naomi en tu navegador de Linux Mint!")
