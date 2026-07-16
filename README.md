<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Corrupción en el Sector Privado Peruano | Análisis y Soluciones</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.8/dist/chart.umd.min.js"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#0F2B4A',
                        secondary: '#165DFF',
                        accent: '#FF7D00',
                        dark: '#0A192F',
                        light: '#F8FAFC',
                        soft: '#E8F0FC'
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style>
        html { scroll-behavior: smooth; }
        .text-gradient {
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            background-image: linear-gradient(to right, #165DFF, #FF7D00);
        }
        .card-hover { transition: all 0.3s ease; }
        .card-hover:hover { transform: translateY(-6px); box-shadow: 0 12px 28px rgba(22, 93, 255, 0.18); }
        .fade-in { opacity: 0; transform: translateY(25px); transition: all 0.8s ease; }
        .fade-in.visible { opacity: 1; transform: translateY(0); }
        .stat-box { background: linear-gradient(145deg, #ffffff, #f1f5f9); border-left: 5px solid #165DFF; }
        .stat-box-accent { border-left: 5px solid #FF7D00; }
        .stat-box-dark { border-left: 5px solid #0F2B4A; }
        .section-divider { height: 4px; background: linear-gradient(90deg, #165DFF, #FF7D00); border-radius: 2px; }
        .interactive-card { cursor: pointer; transition: all 0.3s ease; }
        .interactive-card:hover { background: #E8F0FC; transform: scale(1.02); }
        .progress-bar { height: 10px; background: #e2e8f0; border-radius: 5px; overflow: hidden; }
        .progress-fill { height: 100%; border-radius: 5px; transition: width 1.5s ease-out; width: 0; }
        .tab-content { display: none; }
        .tab-content.active { display: block; animation: fadeIn 0.4s ease; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
    </style>
</head>
<body class="bg-light text-dark font-sans">

    <!-- Barra de Navegación Fija -->
    <nav class="sticky top-0 z-50 bg-white/95 backdrop-blur shadow-md">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <div class="font-bold text-2xl text-primary">
                <span class="text-accent">TRANSPARENCIA</span> PERÚ
            </div>
            <div class="hidden lg:flex gap-6 text-sm font-medium">
                <a href="#inicio" class="hover:text-secondary">Inicio</a>
                <a href="#problema" class="hover:text-secondary">El Problema</a>
                <a href="#causas" class="hover:text-secondary">Causas</a>
                <a href="#graficas" class="hover:text-secondary">Datos y Gráficas</a>
                <a href="#consecuencias" class="hover:text-secondary">Consecuencias</a>
                <a href="#luchar" class="hover:text-secondary">¿Cómo Luchar?</a>
                <a href="#soluciones" class="hover:text-secondary">Soluciones</a>
            </div>
        </div>
    </nav>

    <!-- SECCIÓN 1: INICIO -->
    <section id="inicio" class="min-h-screen flex items-center py-24 bg-gradient-to-br from-primary/10 via-soft to-white">
        <div class="container mx-auto px-6">
            <div class="max-w-5xl mx-auto text-center fade-in">
                <h1 class="text-[clamp(2.8rem,7vw,4.5rem)] font-bold mb-8 leading-tight">
                    La Corrupción en el <span class="text-gradient">Sector Privado Peruano</span>
                </h1>
                <p class="text-[clamp(1.2rem,2.5vw,1.5rem)] text-gray-700 mb-12 leading-relaxed">
                    Análisis profundo, datos visuales, y herramientas interactivas para entender y combatir esta problemática que frena el desarrollo de nuestro país.
                </p>
                <div class="flex flex-wrap justify-center gap-4">
                    <a href="#graficas" class="bg-secondary text-white px-10 py-4 rounded-xl font-semibold shadow-lg hover:shadow-secondary/30 transition-all">Ver Datos Visuales</a>
                    <a href="#luchar" class="bg-accent text-white px-10 py-4 rounded-xl font-semibold hover:bg-accent/90 transition-all">¿Cómo podemos actuar?</a>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN 2: EL PROBLEMA -->
    <section id="problema" class="py-24">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto text-center mb-20 fade-in">
                <h2 class="text-[clamp(2rem,4vw,3rem)] font-bold mb-6">El Problema en Profundidad</h2>
                <div class="section-divider w-32 mx-auto mb-8"></div>
                <p class="text-lg text-gray-700 leading-relaxed">
                    En el sector privado peruano, existe una brecha marcada entre la normativa escrita y la práctica real, además de escasez de información cuantitativa detallada.
                </p>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-2xl shadow-sm card-hover fade-in">
                    <i class="fa fa-balance-scale text-3xl text-secondary mb-4"></i>
                    <h3 class="text-xl font-bold mb-4">Conducta y Cultura</h3>
                    <p class="text-gray-700">Normalización de conductas irregulares y códigos de ética que no se aplican.</p>
                </div>
                <div class="bg-white p-8 rounded-2xl shadow-sm card-hover fade-in delay-1">
                    <i class="fa fa-line-chart text-3xl text-accent mb-4"></i>
                    <h3 class="text-xl font-bold mb-4">Presión y Conflictos</h3>
                    <p class="text-gray-700">Presión por metas y conflictos de interés no resueltos.</p>
                </div>
                <div class="bg-white p-8 rounded-2xl shadow-sm card-hover fade-in delay-2">
                    <i class="fa fa-shield text-3xl text-primary mb-4"></i>
                    <h3 class="text-xl font-bold mb-4">Denuncia e Impunidad</h3>
                    <p class="text-gray-700">Temor a represalias y canales de denuncia inoperantes.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN 3: CAUSAS RAÍZ -->
    <section id="causas" class="py-24 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto text-center mb-20 fade-in">
                <h2 class="text-[clamp(2rem,4vw,3rem)] font-bold mb-6">Causas Raíz</h2>
                <div class="section-divider w-32 mx-auto mb-8"></div>
            </div>
            <div class="grid md:grid-cols-2 gap-10">
                <div class="bg-white p-10 rounded-2xl shadow-sm card-hover fade-in">
                    <h3 class="text-2xl font-bold text-secondary mb-6">Factores Culturales</h3>
                    <ul class="space-y-3 text-gray-700">
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-accent mt-1"></i> Normalización de lo irregular</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-accent mt-1"></i> Falta de ejemplo desde la dirección</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-accent mt-1"></i> Resultados por encima de la ética</li>
                    </ul>
                </div>
                <div class="bg-white p-10 rounded-2xl shadow-sm card-hover fade-in delay-1">
                    <h3 class="text-2xl font-bold text-secondary mb-6">Factores Estructurales</h3>
                    <ul class="space-y-3 text-gray-700">
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-accent mt-1"></i> Cumplimiento solo en papel</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-accent mt-1"></i> Incentivos mal diseñados</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-accent mt-1"></i> Conflictos de interés no gestionados</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- 📊 SECCIÓN 4: GRÁFICAS Y DATOS INTERACTIVOS -->
    <section id="graficas" class="py-24">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto text-center mb-20 fade-in">
                <h2 class="text-[clamp(2rem,4vw,3rem)] font-bold mb-6">📊 Datos y Estadísticas Visuales</h2>
                <div class="section-divider w-32 mx-auto mb-8"></div>
            </div>

            <div class="grid md:grid-cols-2 gap-10 mb-16">
                <!-- Gráfico Circular -->
                <div class="bg-white p-8 rounded-2xl shadow-sm fade-in">
                    <h3 class="text-xl font-semibold text-center mb-6">¿Por qué no se denuncia?</h3>
                    <canvas id="graficoCircular" height="280"></canvas>
                </div>
                <!-- Gráfico de Barras -->
                <div class="bg-white p-8 rounded-2xl shadow-sm fade-in delay-1">
                    <h3 class="text-xl font-semibold text-center mb-6">Impacto estimado en empresas (%)</h3>
                    <canvas id="graficoBarras" height="280"></canvas>
                </div>
            </div>

            <!-- Barras de Progreso Interactivas -->
            <div class="bg-white p-10 rounded-2xl shadow-sm fade-in">
                <h3 class="text-xl font-semibold mb-8 text-center">Indicadores Clave del Sector Privado Peruano</h3>
                <div class="space-y-8">
                    <div>
                        <div class="flex justify-between mb-2 font-medium">
                            <span>Cumplimiento solo formal de normas</span>
                            <span class="text-secondary font-bold">72%</span>
                        </div>
                        <div class="progress-bar"><div class="progress-fill bg-secondary" data-width="72"></div></div>
                    </div>
                    <div>
                        <div class="flex justify-between mb-2 font-medium">
                            <span>Presión para actuar sin ética</span>
                            <span class="text-accent font-bold">65%</span>
                        </div>
                        <div class="progress-bar"><div class="progress-fill bg-accent" data-width="65"></div></div>
                    </div>
                    <div>
                        <div class="flex justify-between mb-2 font-medium">
                            <span>Miedo a represalias al denunciar</span>
                            <span class="text-primary font-bold">58%</span>
                        </div>
                        <div class="progress-bar"><div class="progress-fill bg-primary" data-width="58"></div></div>
                    </div>
                    <div>
                        <div class="flex justify-between mb-2 font-medium">
                            <span>Empresas sin canales de denuncia seguros</span>
                            <span class="text-purple-600 font-bold">60%</span>
                        </div>
                        <div class="progress-bar"><div class="progress-fill bg-purple-600" data-width="60"></div></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN 5: CONSECUENCIAS -->
    <section id="consecuencias" class="py-24 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto text-center mb-20 fade-in">
                <h2 class="text-[clamp(2rem,4vw,3rem)] font-bold mb-6">Consecuencias</h2>
                <div class="section-divider w-32 mx-auto mb-8"></div>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-gradient-to-br from-secondary/10 to-secondary/5 p-10 rounded-2xl card-hover fade-in">
                    <h3 class="text-xl font-bold text-secondary mb-4">Económicas</h3>
                    <p>Pérdidas, competencia desleal, menos inversión.</p>
                </div>
                <div class="bg-gradient-to-br from-accent/10 to-accent/5 p-10 rounded-2xl card-hover fade-in delay-1">
                    <h3 class="text-xl font-bold text-accent mb-4">Sociales</h3>
                    <p>Desconfianza, mal clima laboral, daño al país.</p>
                </div>
                <div class="bg-gradient-to-br from-primary/10 to-primary/5 p-10 rounded-2xl card-hover fade-in delay-2">
                    <h3 class="text-xl font-bold text-primary mb-4">Estructurales</h3>
                    <p>Debilidad organizacional, riesgo constante.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 🎯 SECCIÓN 6: ¿CÓMO PODEMOS LUCHAR? (INTERACTIVA) -->
    <section id="luchar" class="py-24 bg-gradient-to-br from-primary/5 to-secondary/5">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto text-center mb-20 fade-in">
                <h2 class="text-[clamp(2rem,4vw,3rem)] font-bold mb-6">🎯 ¿Cómo podemos luchar contra esto?</h2>
                <div class="section-divider w-32 mx-auto mb-8"></div>
                <p class="text-lg text-gray-700">Haz clic en cada área para ver acciones concretas:</p>
            </div>

            <!-- Pestañas Interactivas -->
            <div class="flex flex-wrap justify-center gap-3 mb-10 fade-in">
                <button class="tab-btn bg-secondary text-white px-6 py-3 rounded-lg font-medium" data-tab="individual">Como Persona</button>
                <button class="tab-btn bg-white text-primary border px-6 py-3 rounded-lg font-medium" data-tab="empresa">En la Empresa</button>
                <button class="tab-btn bg-white text-primary border px-6 py-3 rounded-lg font-medium" data-tab="colectivo">Juntos y Sociedad</button>
            </div>

            <!-- Contenido de Pestañas -->
            <div class="max-w-4xl mx-auto">
                <div id="individual" class="tab-content active bg-white p-8 rounded-2xl shadow-sm fade-in">
                    <h3 class="text-2xl font-bold text-secondary mb-4">💪 Acciones Individuales</h3>
                    <ul class="space-y-3 text-gray-700">
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Actúa con integridad en todo lo que hagas, sin excepciones.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Conoce tus derechos y los canales de denuncia disponibles.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> No participes ni justifiques conductas que sabes que son incorrectas.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Apoya y respeta a quienes se atreven a denunciar con valentía.</li>
                    </ul>
                </div>
                <div id="empresa" class="tab-content bg-white p-8 rounded-2xl shadow-sm fade-in">
                    <h3 class="text-2xl font-bold text-accent mb-4">🏢 Acciones en la Empresa</h3>
                    <ul class="space-y-3 text-gray-700">
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Crea canales de denuncia reales, seguros y confidenciales.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Alinea recompensas con conducta ética, no solo con resultados.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> La alta dirección debe dar el ejemplo visiblemente.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Capacita y escucha a tu equipo constantemente.</li>
                    </ul>
                </div>
                <div id="colectivo" class="tab-content bg-white p-8 rounded-2xl shadow-sm fade-in">
                    <h3 class="text-2xl font-bold text-primary mb-4">🤝 Acciones Colectivas</h3>
                    <ul class="space-y-3 text-gray-700">
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Exige transparencia a empresas y autoridades.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Apoya iniciativas y organismos que promueven la ética.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Difunde información correcta y combate la normalización.</li>
                        <li class="flex items-start gap-3"><i class="fa fa-check-circle text-green-500 mt-1"></i> Rechaza activamente cualquier práctica corrupta en tu entorno.</li>
                    </ul>
                </div>
            </div>

            <!-- Tarjetas Interactivas -->
            <div class="grid md:grid-cols-3 gap-6 mt-16">
                <div class="interactive-card bg-white p-6 rounded-xl shadow-sm text-center" onclick="alert('¡Recuerda! La honestidad construye confianza y confianza genera progreso.')">
                    <i class="fa fa-lightbulb-o text-3xl text-accent mb-4"></i>
                    <h4 class="font-bold">Reflexiona</h4>
                    <p class="text-sm text-gray-600">¿Qué harías tú en una situación difícil?</p>
                </div>
                <div class="interactive-card bg-white p-6 rounded-xl shadow-sm text-center" onclick="alert('En Perú puedes consultar con Transparencia Internacional, Contraloría o Defensoría del Pueblo.')">
                    <i class="fa fa-info-circle text-3xl text-secondary mb-4"></i>
                    <h4 class="font-bold">Infórmate</h4>
                    <p class="text-sm text-gray-600">Conoce las instituciones que te protegen.</p>
                </div>
                <div class="interactive-card bg-white p-6 rounded-xl shadow-sm text-center" onclick="alert('¡El cambio empieza por cada uno de nosotros! Tu compromiso cuenta mucho.')">
                    <i class="fa fa-heart text-3xl text-red-500 mb-4"></i>
                    <h4 class="font-bold">Comprométete</h4>
                    <p class="text-sm text-gray-600">Sé parte de la solución.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN 7: SOLUCIONES -->
    <section id="soluciones" class="py-24 bg-primary text-white">
        <div class="container mx-auto px-6">
            <div class="max-w-4xl mx-auto text-center mb-20 fade-in">
                <h2 class="text-[clamp(2rem,4vw,3rem)] font-bold mb-6">Soluciones Integrales</h2>
                <div class="section-divider w-32 mx-auto mb-8"></div>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="bg-white/10 p-6 rounded-xl card-hover fade-in"><h4 class="font-bold mb-2">Liderazgo Ejemplo</h4><p class="text-sm opacity-90">Coherencia total desde arriba</p></div>
                <div class="bg-white/10 p-6 rounded-xl card-hover fade-in delay-1"><h4 class="font-bold mb-2">Denuncia Segura</h4><p class="text-sm opacity-90">Protección real a quien habla</p></div>
                <div class
