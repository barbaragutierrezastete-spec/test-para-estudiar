# test-para-estudiar
test para cuando necesite ayuda con un tema
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🧁 Test de Pastelería y Repostería</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }
        body { background: linear-gradient(135deg, #fdf2e9, #fce4d6); min-height: 100vh; padding: 2rem; }
        .container { max-width: 900px; margin: 0 auto; }
        header { text-align: center; margin-bottom: 3rem; }
        h1 { color: #8b4513; font-size: 2rem; margin-bottom: 0.5rem; }
        .subtitulo { color: #a06030; font-size: 1.1rem; }
        
        /* Navegación */
        nav { background: white; border-radius: 12px; padding: 1.5rem; margin-bottom: 2rem; box-shadow: 0 4px 12px rgba(0,0,0,0.08); }
        nav h2 { color: #5a3817; margin-bottom: 1rem; font-size: 1.2rem; }
        .menu { list-style: none; }
        .menu li { margin: 0.8rem 0; }
        .menu a { display: block; padding: 0.9rem 1.2rem; background: linear-gradient(135deg, #fff3e8, #ffe8d4); color: #8b4513; text-decoration: none; border-radius: 10px; font-weight: 600; transition: all 0.3s; border-left: 4px solid #e67e22; }
        .menu a:hover { transform: translateX(5px); background: linear-gradient(135deg, #ffe8d4, #ffd4b0); }
        
        /* Sección Test */
        .seccion-test { background: white; border-radius: 16px; padding: 2.5rem; box-shadow: 0 8px 24px rgba(0,0,0,0.1); display: none; }
        .seccion-test.activa { display: block; }
        .volver { display: inline-block; margin-bottom: 1.5rem; color: #e67e22; text-decoration: none; font-weight: 600; cursor: pointer; }
        .volver:hover { text-decoration: underline; }
        
        .puntuacion { text-align: center; font-size: 1.3rem; font-weight: bold; color: #2d5016; margin-bottom: 2rem; padding: 1rem; background: #f0f9e6; border-radius: 12px; display: none; }
        .pregunta { margin-bottom: 2rem; padding: 1.5rem; border-radius: 12px; background: #fef6ef; border-left: 4px solid #e67e22; }
        .enunciado { font-weight: 600; color: #5a3817; margin-bottom: 1rem; font-size: 1.05rem; }
        .alternativa { display: block; padding: 0.7rem 1rem; margin: 0.5rem 0; border-radius: 8px; cursor: pointer; transition: all 0.3s; border: 2px solid transparent; }
        .alternativa:hover { background: #ffe8d4; border-color: #f5b88c; }
        input[type="radio"] { margin-right: 0.7rem; transform: scale(1.1); }
        .correcta { background: #e6ffd4; border-color: #4caf50; color: #206020; }
        .incorrecta { background: #ffe4e4; border-color: #e74c3c; color: #a02020; }
        .explicacion { margin-top: 0.8rem; padding: 0.8rem; background: #fff8dc; border-radius: 6px; font-size: 0.9rem; color: #6b4226; display: none; }
        .botones { display: flex; gap: 1rem; justify-content: center; margin-top: 2rem; flex-wrap: wrap; }
        button { padding: 0.9rem 2rem; border: none; border-radius: 10px; font-size: 1rem; font-weight: 600; cursor: pointer; transition: transform 0.2s, box-shadow 0.2s; }
        button:hover { transform: translateY(-2px); box-shadow: 0 4px 12px rgba(0,0,0,0.15); }
        .enviar { background: linear-gradient(135deg, #e67e22, #d35400); color: white; }
        .reiniciar { background: #e0e0e0; color: #444; }
        .respondido { pointer-events: none; }
        
        footer { text-align: center; margin-top: 3rem; color: #a06030; font-size: 0.9rem; }
    </style>
</head>
<body>
    <div class="container">
        <!-- Página de Inicio -->
        <header id="pagina-inicio">
            <h1>🧁 Academia de Pastelería y Repostería</h1>
            <p class="subtitulo">Tu espacio para practicar y aprender con tests interactivos</p>
        </header>

        <!-- Menú de Tests -->
        <nav id="menu-principal">
            <h2>📋 Elige un test para comenzar</h2>
            <ul class="menu">
                <li><a href="#" data-test="test1">📝 Test 1: Fundamentos Básicos</a></li>
                <!-- Aquí agregaré automáticamente los nuevos tests que pidas -->
            </ul>
        </nav>

        <!-- Test 1: Fundamentos -->
        <section class="seccion-test" id="test1">
            <span class="volver" onclick="volverMenu()">← Volver al menú</span>
            <h2 style="text-align:center; color:#8b4513; margin-bottom:0.5rem;">Test 1: Fundamentos de Pastelería y Repostería</h2>
            <p style="text-align:center; color:#666; margin-bottom:2rem;">Responde las 15 preguntas y comprueba tus conocimientos.</p>
            
            <div class="puntuacion" id="puntuacion1"></div>
            <form class="form-test" data-id="1">
                <!-- Pregunta 1 -->
                <div class="pregunta">
                    <p class="enunciado">1. ¿Qué característica diferencia a la pastelería de la cocción culinaria general?</p>
                    <label class="alternativa"><input type="radio" name="p1" value="a"> a) Se usan solo ingredientes dulces</label>
                    <label class="alternativa"><input type="radio" name="p1" value="b"> b) Las proporciones y el pesaje definen la estructura final</label>
                    <label class="alternativa"><input type="radio" name="p1" value="c"> c) No se requiere controlar la temperatura</label>
                    <label class="alternativa"><input type="radio" name="p1" value="d"> d) Solo se elaboran postres fríos</label>
                    <div class="explicacion">✅ Correcta: b. En pastelería, las cantidades exactas definen la estructura del producto.</div>
                </div>
                <!-- Pregunta 2 -->
                <div class="pregunta">
                    <p class="enunciado">2. ¿Cuál es la función principal de la harina?</p>
                    <label class="alternativa"><input type="radio" name="p2" value="a"> a) Aportar dulzor y color</label>
                    <label class="alternativa"><input type="radio" name="p2" value="b"> b) Aportar estructura mediante almidón y proteínas</label>
                    <label class="alternativa"><input type="radio" name="p2" value="c"> c) Emulsionar grasas y líquidos</label>
                    <label class="alternativa"><input type="radio" name="p2" value="d"> d) Dar brillo a las preparaciones</label>
                    <div class="explicacion">✅ Correcta: b. La harina aporta almidón y proteínas que forman la estructura de masas y batidos.</div>
                </div>
                <!-- Pregunta 3 -->
                <div class="pregunta">
                    <p class="enunciado">3. En el cremado de mantequilla, ¿cuál es la temperatura ideal aproximada?</p>
                    <label class="alternativa"><input type="radio" name="p3" value="a"> a) 10–12 °C</label>
                    <label class="alternativa"><input type="radio" name="p3" value="b"> b) 18–21 °C</label>
                    <label class="alternativa"><input type="radio" name="p3" value="c"> c) 30–35 °C</label>
                    <label class="alternativa"><input type="radio" name="p3" value="d"> d) Más de 40 °C</label>
                    <div class="explicacion">✅ Correcta: b. La mantequilla debe estar plástica pero no derretida; el rango ideal es 18–21 °C.</div>
                </div>
                <!-- Pregunta 4 -->
                <div class="pregunta">
                    <p class="enunciado">4. ¿Qué ocurre si se mezcla en exceso la harina una vez hidratada?</p>
                    <label class="alternativa"><input type="radio" name="p4" value="a"> a) La masa queda más suave</label>
                    <label class="alternativa"><input type="radio" name="p4" value="b"> b) Se desarrolla gluten en exceso y el producto resulta compacto</label>
                    <label class="alternativa"><input type="radio" name="p4" value="c"> c) Aumenta el volumen del bizcocho</label>
                    <label class="alternativa"><input type="radio" name="p4" value="d"> d) No hay cambios significativos</label>
                    <div class="explicacion">✅ Correcta: b. El mezclado prolongado favorece el desarrollo del gluten, dando un producto denso.</div>
                </div>
                <!-- Pregunta 5 -->
                <div class="pregunta">
                    <p class="enunciado">5. La fórmula de la masa mürbe o 1-2-3 corresponde a:</p>
                    <label class="alternativa"><input type="radio" name="p5" value="a"> a) 1 parte de harina : 2 de azúcar : 3 de grasa</label>
                    <label class="alternativa"><input type="radio" name="p5" value="b"> b) 1 parte de azúcar : 2 de grasa : 3 de harina</label>
                    <label class="alternativa"><input type="radio" name="p5" value="c"> c) 1 parte de grasa : 2 de harina : 3 de azúcar</label>
                    <label class="alternativa"><input type="radio" name="p5" value="d"> d) 1 huevo : 2 de harina : 3 de azúcar</label>
                    <div class="explicacion">✅ Correcta: b. La proporción tradicional es 1 de azúcar, 2 de grasa y 3 de harina.</div>
                </div>
                <!-- Pregunta 6 -->
                <div class="pregunta">
                    <p class="enunciado">6. ¿Qué punto de almíbar se alcanza aproximadamente a 112–116 °C?</p>
                    <label class="alternativa"><input type="radio" name="p6" value="a"> a) Hilo</label>
                    <label class="alternativa"><input type="radio" name="p6" value="b"> b) Bola blanda</label>
                    <label class="alternativa"><input type="radio" name="p6" value="c"> c) Bola firme</label>
                    <label class="alternativa"><input type="radio" name="p6" value="d"> d) Caramelo</label>
                    <div class="explicacion">✅ Correcta: b. 112–116 °C corresponde al punto de bola blanda.</div>
                </div>
                <!-- Pregunta 7 -->
                <div class="pregunta">
                    <p class="enunciado">7. ¿Cuál de los siguientes merengues se prepara con almíbar caliente?</p>
                    <label class="alternativa"><input type="radio" name="p7" value="a"> a) Francés</label>
                    <label class="alternativa"><input type="radio" name="p7" value="b"> b) Suizo</label>
                    <label class="alternativa"><input type="radio" name="p7" value="c"> c) Italiano</label>
                    <label class="alternativa"><input type="radio" name="p7" value="d"> d) Todos los anteriores</label>
                    <div class="explicacion">✅ Correcta: c. El merengue italiano incorpora el almíbar caliente sobre las claras en batido.</div>
                </div>
                <!-- Pregunta 8 -->
                <div class="pregunta">
                    <p class="enunciado">8. ¿A qué temperatura debe estar la crema para montarla correctamente?</p>
                    <label class="alternativa"><input type="radio" name="p8" value="a"> a) 10–15 °C</label>
                    <label class="alternativa"><input type="radio" name="p8" value="b"> b) 2–7 °C</label>
                    <label class="alternativa"><input type="radio" name="p8" value="c"> c) Temperatura ambiente</label>
                    <label class="alternativa"><input type="radio" name="p8" value="d"> d) Congelada</label>
                    <div class="explicacion">✅ Correcta: b. La crema debe estar bien fría (2–7 °C) para formar una red estable.</div>
                </div>
                <!-- Pregunta 9 -->
                <div class="pregunta">
                    <p class="enunciado">9. ¿Qué proporción de hidratación se usa para la gelatina en polvo?</p>
                    <label class="alternativa"><input type="radio" name="p9" value="a"> a) 1 parte de gelatina por 2 partes de agua</label>
                    <label class="alternativa"><input type="radio" name="p9" value="b"> b) 1 parte de gelatina por 5 partes de agua</label>
                    <label class="alternativa"><input type="radio" name="p9" value="c"> c) 1 parte de gelatina por 10 partes de agua</label>
                    <label class="alternativa"><input type="radio" name="p9" value="d"> d) Cantidad de agua según el gusto</label>
                    <div class="explicacion">✅ Correcta: b. La proporción estándar de hidratación es 1:5.</div>
                </div>
                <!-- Pregunta 10 -->
                <div class="pregunta">
                    <p class="enunciado">10. ¿Cuál es la diferencia principal entre crema pastelera y crema inglesa?</p>
                    <label class="alternativa"><input type="radio" name="p10" value="a"> a) La crema inglesa lleva más azúcar</label>
                    <label class="alternativa"><input type="radio" name="p10" value="b"> b) La crema pastelera usa almidón como espesante; la inglesa no</label>
                    <label class="alternativa"><input type="radio" name="p10" value="c"> c) La crema inglesa se cocina a mayor temperatura</label>
                    <label class="alternativa"><input type="radio" name="p10" value="d"> d) No hay diferencia significativa</label>
                    <div class="explicacion">✅ Correcta: b. La pastelera se espesa con almidón; la inglesa por coagulación de yemas.</div>
                </div>
                <!-- Pregunta 11 -->
                <div class="pregunta">
                    <p class="enunciado">11. ¿Cómo se forma la ganache?</p>
                    <label class="alternativa"><input type="radio" name="p11" value="a"> a) Herviendo leche con azúcar y mantequilla</label>
                    <label class="alternativa"><input type="radio" name="p11" value="b"> b) Mezclando chocolate con crema caliente</label>
                    <label class="alternativa"><input type="radio" name="p11" value="c"> c) Derritiendo chocolate con agua</label>
                    <label class="alternativa"><input type="radio" name="p11" value="d"> d) Mezclando chocolate con mantequilla fría</label>
                    <div class="explicacion">✅ Correcta: b. La ganache es una emulsión de chocolate y crema caliente.</div>
                </div>
                <!-- Pregunta 12 -->
                <div class="pregunta">
                    <p class="enunciado">12. Para chocolate negro, la temperatura de trabajo tras fundir es aproximadamente:</p>
                    <label class="alternativa"><input type="radio" name="p12" value="a"> a) 20–22 °C</label>
                    <label class="alternativa"><input type="radio" name="p12" value="b"> b) 29–30 °C</label>
                    <label class="alternativa"><input type="radio" name="p12" value="c"> c) 31–32 °C</label>
                    <label class="alternativa"><input type="radio" name="p12" value="d"> d) 40–42 °C</label>
                    <div class="explicacion">✅ Correcta: c. El chocolate negro se trabaja idealmente a 31–32 °C.</div>
                </div>
                <!-- Pregunta 13 -->
                <div class="pregunta">
                    <p class="enunciado">13. ¿Qué técnica consiste en igualar gradualmente la temperatura de dos mezclas antes de unirlas?</p>
                    <label class="alternativa"><input type="radio" name="p13" value="a"> a) Napar</label>
                    <label class="alternativa"><input type="radio" name="p13" value="b"> b) Templar</label>
                    <label class="alternativa"><input type="radio" name="p13" value="c"> c) Escaldar</label>
                    <label class="alternativa"><input type="radio" name="p13" value="d"> d) Emulsionar</label>
                    <div class="explicacion">✅ Correcta: b. Templar es igualar temperaturas para evitar cambios bruscos.</div>
                </div>
                <!-- Pregunta 14 -->
                <div class="pregunta">
                    <p class="enunciado">14. La pâte à choux adquiere volumen durante la cocción principalmente por:</p>
                    <label class="alternativa"><input type="radio" name="p14" value="a"> a) La levadura</label>
                    <label class="alternativa"><input type="radio" name="p14" value="b"> b) El vapor de agua</label>
                    <label class="alternativa"><input type="radio" name="p14" value="c"> c) El bicarbonato</label>
                    <label class="alternativa"><input type="radio" name="p14" value="d"> d) El aire batido</label>
                    <div class="explicacion">✅ Correcta: b. El agua se convierte en vapor y expande la estructura.</div>
                </div>
                <!-- Pregunta 15 -->
                <div class="pregunta">
                    <p class="enunciado">15. ¿Cuál de las siguientes afirmaciones es correcta?</p>
                    <label class="alternativa"><input type="radio" name="p15" value="a"> a) Gelatina y agar-agar pueden sustituirse en igual cantidad</label>
                    <label class="alternativa"><input type="radio" name="p15" value="b"> b) Un exceso de agente leudante garantiza mayor volumen</label>
                    <label class="alternativa"><input type="radio" name="p15" value="c"> c) El pesaje es más preciso que medir por volumen en pastelería</label>
                    <label class="alternativa"><input type="radio" name="p15" value="d"> d) Las preparaciones con huevo pueden conservarse a temperatura ambiente</label>
                    <div class="explicacion">✅ Correcta: c. Pesar es más exacto que usar medidas de volumen.</div>
                </div>
                
                <div class="botones">
                    <button type="submit" class="enviar">✅ Enviar respuestas</button>
                    <button type="reset" class="reiniciar">🔄 Reiniciar test</button>
                </div>
            </form>
        </section>

        <footer>
            <p>🍰 Tu espacio de aprendizaje en Pastelería — Todos los tests se irán agregando aquí</p>
        </footer>
    </div>

    <script>
        // Base de respuestas
        const respuestasTests = {
            test1: {
                resp: {p1:'b',p2:'b',p3:'b',p4:'b',p5:'b',p6:'b',p7:'c',p8:'b',p9:'b',p10:'b',p11:'b',p12:'c',p13:'b',p14:'b',p15:'c'},
                total: 15
            }
        };

        // Navegación
        document.querySelectorAll('.menu a').forEach(enlace => {
            enlace.addEventListener('click', function(e) {
                e.preventDefault();
                const idTest = this.getAttribute('data-test');
                document.querySelectorAll('.seccion-test').forEach(t => t.classList.remove('activa'));
                document.getElementById(idTest).classList.add('activa');
                document.getElementById('pagina-inicio').style.display = 'none';
                document.getElementById('menu-principal').style.display = 'none';
            });
        });

        function volverMenu() {
            document.querySelectorAll('.seccion-test').forEach(t => t.classList.remove('activa'));
            document.getElementById('pagina-inicio').style.display = 'block';
            document.getElementById('menu-principal').style.display = 'block';
        }

        // Procesar tests
        document.querySelectorAll('.form-test').forEach(form => {
            form.addEventListener('submit', function(e) {
                e.preventDefault();
                const id = this.getAttribute('data-id');
                const datos = respuestasTests[`test${id}`];
                const cajaPuntuacion = document.getElementById(`puntuacion${id}`);
                let aciertos = 0;

                for (const [nombre, correcta] of Object.entries(datos.resp)) {
                    const pregunta = this.querySelector(`input[name="${nombre}"]`).closest('.pregunta');
                    const seleccionada = pregunta.querySelector(`input:checked`);
                    const explicacion = pregunta.querySelector('.explicacion');
                    
                    pregunta.classList.add('respondido');
                    pregunta.querySelectorAll('.alternativa').forEach(a => a.classList.remove('correcta','incorrecta'));
                    explicacion.style.display = 'none';

                    if (seleccionada) {
                        const valor = seleccionada.value;
                        pregunta.querySelector(`input[value="${correcta}"]`).parentElement.classList.add('correcta');
                        if (valor === correcta) aciertos++;
                        else seleccionada.parentElement.classList.add('incorrecta');
                        explicacion.style.display = 'block';
                    }
                }

                cajaPuntuacion.style.display = 'block';
                cajaPuntuacion.innerHTML = `🏆 Puntuación: ${aciertos} de ${datos.total} (${Math.round(aciertos/datos.total*100)}%)`;
                if (aciertos === datos.total) cajaPuntuacion.innerHTML += '<br>🎉 ¡Excelente! Dominas los fundamentos.';
                else if (aciertos >= 12) cajaPuntuacion.innerHTML += '<br>👏 ¡Muy buen trabajo!';
                else if (aciertos >= 9) cajaPuntuacion.innerHTML += '<br>💪 Bien hecho, puedes repasar algunos puntos.';
                else cajaPuntuacion.innerHTML += '<br>📖 Te recomiendo revisar el material nuevamente.';
            });

            form.addEventListener('reset', function() {
                setTimeout(() => {
                    const id = this.getAttribute('data-id');
                    document.getElementById(`puntuacion${id}`).style.display = 'none';
                    this.querySelectorAll('.pregunta').forEach(p => {
                        p.classList.remove('respondido');
                        p.querySelectorAll('.alternativa').forEach(a => a.classList.remove('correcta','incorrecta'));
                        p.querySelector('.explicacion').style.display = 'none';
                    });
                }, 10);
            });
        });
    </script>
</body>
</html>
