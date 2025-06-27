# apresentacao-ufsj
Documentos eApresentações PROEN-UFSJ
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infográfico: Descubra a UFSJ</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;900&display=swap" rel="stylesheet">
    <style>
        /* Cor da paleta: Cinza, Tons de Vermelho e Branco */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f3f4f6; /* Tom de cinza bem claro para o fundo */
        }
        .chart-container {
            position: relative;
            margin: auto;
            height: 40vh;
            width: 100%;
            max-width: 600px;
        }
        @media (max-width: 768px) {
            .chart-container {
                height: 50vh;
            }
        }
        .collapsible-header {
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem;
            background-color: #e5e7eb; /* Tom de cinza mais escuro para o cabeçalho */
            border-bottom: 1px solid #d1d5db; /* Tom de cinza para a borda */
            border-radius: 0.5rem;
            margin-bottom: 0.5rem;
            font-weight: bold;
            color: #C70039; /* Texto em vermelho escuro */
            transition: background-color 0.2s ease-in-out;
        }
        .collapsible-header:hover {
            background-color: #d1d5db; /* Tom de cinza no hover */
        }
        .collapsible-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
        }
        .collapsible-content.open {
            max-height: 500px; /* Ajuste com base na altura esperada do conteúdo */
            padding: 1rem;
            background-color: #ffffff;
            border: 1px solid #d1d5db; /* Tom de cinza para a borda */
            border-top: none;
            border-radius: 0 0 0.5rem 0.5rem;
        }
        .collapsible-header .arrow {
            transition: transform 0.3s ease-out;
        }
        .collapsible-header.active .arrow {
            transform: rotate(90deg);
        }
    </style>
</head>
<body class="text-gray-800">
    <!-- Cor da paleta: Cinza, Tons de Vermelho e Branco -->

    <header class="bg-[#C70039] text-white text-center py-8 px-4"> <!-- Banner inicial vermelho -->
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e4/UFSJ_logo_2018.jpg/180px-UFSJ_logo_2018.jpg" alt="[Imagem do Logo da UFSJ]" class="mx-auto mb-4 rounded-md shadow-md">
        <h1 class="text-4xl md:text-6xl font-black uppercase tracking-wide">Descubra a UFSJ</h1>
        <p class="mt-4 text-lg md:text-xl font-light text-white">Sua Universidade Pública, Gratuita e de Qualidade</p>
    </header>

    <main class="container mx-auto p-4 md:p-8">

        <section id="hero-image" class="my-8">
            <img src="https://ufsj.edu.br/ascom/fotos_csa/fachada_horizontal.jpg" alt="[Imagem do Campus Santo Antônio da UFSJ]" class="w-full h-auto rounded-xl shadow-lg object-cover">
        </section>

        <section id="overview" class="my-12">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center text-gray-800">
                <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-[#C70039]"> <!-- Borda em vermelho escuro -->
                    <p class="text-6xl font-extrabold text-gray-800">6</p>
                    <h3 class="mt-2 text-xl font-bold">Campi</h3>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-[#C70039]"> <!-- Borda em vermelho escuro -->
                    <p class="text-6xl font-extrabold text-gray-800">52</p>
                    <h3 class="mt-2 text-xl font-bold">Cursos de Graduação</h3>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-[#C70039]"> <!-- Borda em vermelho escuro -->
                    <p class="text-6xl font-extrabold text-gray-800">1954</p>
                    <h3 class="mt-2 text-xl font-bold">Início da História</h3>
                </div>
            </div>
        </section>
        
        <section id="history" class="my-16">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12 text-[#C70039]">Uma Trajetória de Crescimento</h2> <!-- Título vermelho -->
            <div class="relative wrap overflow-hidden p-10 h-full">
                <div class="border-2-2 absolute border-opacity-20 border-gray-300 h-full border" style="left: 50%"></div> <!-- Linha cinza claro -->
                <div class="mb-8 flex justify-between items-center w-full right-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-[#FF5733] shadow-xl w-8 h-8 rounded-full"> <!-- Círculo laranja/vermelho -->
                        <h1 class="mx-auto font-semibold text-lg text-white">1</h1>
                    </div>
                    <div class="order-1 bg-white rounded-lg shadow-xl w-5/12 px-6 py-4">
                        <h3 class="font-bold text-gray-800 text-xl">1954</h3>
                        <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">Criação das faculdades pioneiras de Filosofia, Letras e Pedagogia.</p>
                    </div>
                </div>
                <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-[#FF5733] shadow-xl w-8 h-8 rounded-full"> <!-- Círculo laranja/vermelho -->
                        <h1 class="mx-auto text-white font-semibold text-lg">2</h1>
                    </div>
                    <div class="order-1 bg-white rounded-lg shadow-xl w-5/12 px-6 py-4">
                        <h3 class="font-bold text-gray-800 text-xl">1986</h3>
                        <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">Unificação das faculdades (Filosofia, Letras e Pedagogia; Ciências Econômicas, Administrativas e Contábeis; e Engenharia Industrial) para formar a Fundação de Ensino Superior (FUNREI).</p>
                    </div>
                </div>
                <div class="mb-8 flex justify-between items-center w-full right-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-[#FF5733] shadow-xl w-8 h-8 rounded-full"> <!-- Círculo laranja/vermelho -->
                        <h1 class="mx-auto font-semibold text-lg text-white">3</h1>
                    </div>
                    <div class="order-1 bg-white rounded-lg shadow-xl w-5/12 px-6 py-4">
                        <h3 class="font-bold text-gray-800 text-xl">2002</h3>
                        <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">FUNREI é transformada na Universidade Federal de São João del-Rei (UFSJ).</p>
                    </div>
                </div>
                <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-[#FF5733] shadow-xl w-8 h-8 rounded-full"> <!-- Círculo laranja/vermelho -->
                        <h1 class="mx-auto text-white font-semibold text-lg">4</h1>
                    </div>
                    <div class="order-1 bg-white rounded-lg shadow-xl w-5/12 px-6 py-4">
                        <h3 class="font-bold text-gray-800 text-xl">2008</h3>
                        <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">Expansão com novos campi em Divinópolis (CCO) e Ouro Branco (CAP).</p>
                    </div>
                </div>
                <div class="mb-8 flex justify-between items-center w-full right-timeline">
                    <div class="order-1 w-5/12"></div>
                    <div class="z-20 flex items-center order-1 bg-[#FF5733] shadow-xl w-8 h-8 rounded-full"> <!-- Círculo laranja/vermelho -->
                        <h1 class="mx-auto font-semibold text-lg text-white">5</h1>
                    </div>
                    <div class="order-1 bg-white rounded-lg shadow-xl w-5/12 px-6 py-4">
                        <h3 class="font-bold text-gray-800 text-xl">2009</h3>
                        <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">Criação do Campus Sete Lagoas (CSL).</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="courses" class="my-16">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-[#C70039]">Um Universo de Cursos</h2>
            <p class="text-center text-lg max-w-3xl mx-auto mb-12">A UFSJ oferece atualmente **52 cursos de graduação**, cada um com sua vocação e excelência. É importante ressaltar que os cursos de EAD e o curso de Música não estão incluídos no processo seletivo via SISU.</p>
            <div class="bg-white p-4 md:p-8 rounded-xl shadow-lg">
                <h3 class="text-2xl font-bold text-center mb-4">Cursos por Campus</h3>
                <div class="chart-container">
                    <canvas id="coursesByCampusChart"></canvas>
                </div>
                <p class="text-center mt-4 text-sm text-gray-600">Este gráfico mostra a distribuição de alguns dos principais cursos de graduação pelos campi da UFSJ, destacando a diversidade de áreas do conhecimento que a universidade abrange.</p>

                <div class="mt-8">
                    <h4 class="text-xl font-bold text-center mb-4 text-[#C70039]">Conheça os Cursos Detalhados por Campus:</h4> <!-- Título em vermelho escuro -->

                    <div class="mb-4">
                        <div class="collapsible-header" onclick="toggleCollapsible('sjdr-courses')">
                            Campus São João del-Rei (CTAN, CDB, CSA)
                            <span class="arrow">▶</span>
                        </div>
                        <div id="sjdr-courses" class="collapsible-content">
                            <ul class="list-disc list-inside space-y-1">
                                <li class="font-bold text-[#C70039]">Campus Tancredo Neves (CTAN):</li>
                                <ul>
                                    <li>Administração</li>
                                    <li>Arquitetura e Urbanismo</li>
                                    <li>Ciência da Computação</li>
                                    <li>Ciências Contábeis</li>
                                    <li>Comunicação Social (Jornalismo)</li>
                                    <li>Educação Física</li>
                                    <li>Geografia</li>
                                    <li>Música</li>
                                    <li>Artes Aplicadas</li>
                                    <li>Teatro</li>
                                    <li>Zootecnia</li>
                                    <li>Ciências Econômicas</li>
                                </ul>
                                <li class="font-bold text-[#C70039]">Campus Dom Bosco (CDB):</li>
                                <ul>
                                    <li>Biotecnologia</li>
                                    <li>Ciências Biológicas</li>
                                    <li>Filosofia</li>
                                    <li>Física</li>
                                    <li>História</li>
                                    <li>Letras</li>
                                    <li>Medicina</li>
                                    <li>Pedagogia</li>
                                    <li>Psicologia</li>
                                    <li>Química</li>
                                </ul>
                                <li class="font-bold text-[#C70039]">Campus Santo Antônio (CSA):</li>
                                <ul>
                                    <li>Engenharia Elétrica</li>
                                    <li>Engenharia Mecânica</li>
                                    <li>Engenharia de Produção</li>
                                    <li>Matemática</li>
                                </ul>
                            </ul>
                        </div>
                    </div>

                    <div class="mb-4">
                        <div class="collapsible-header" onclick="toggleCollapsible('divinopolis-courses')">
                            Campus Divinópolis (CCO - Dona Lindu)
                            <span class="arrow">▶</span>
                        </div>
                        <div id="divinopolis-courses" class="collapsible-content">
                            <ul class="list-disc list-inside space-y-1">
                                <li>Bioquímica</li>
                                <li>Enfermagem</li>
                                <li>Farmácia</li>
                                <li>Medicina</li>
                            </ul>
                        </div>
                    </div>

                    <div class="mb-4">
                        <div class="collapsible-header" onclick="toggleCollapsible('ourobranco-courses')">
                            Campus Ouro Branco (CAP - Alto Paraopeba)
                            <span class="arrow">▶</span>
                        </div>
                        <div id="ourobranco-courses" class="collapsible-content">
                            <ul class="list-disc list-inside space-y-1">
                                <li>Engenharia Civil</li>
                                <li>Engenharia de Bioprocessos</li>
                                <li>Engenharia de Telecomunicações</li>
                                <li>Engenharia Mecatrônica</li>
                                <li>Engenharia Química</li>
                            </ul>
                        </div>
                    </div>

                    <div class="mb-4">
                        <div class="collapsible-header" onclick="toggleCollapsible('setelagoas-courses')">
                            Campus Sete Lagoas (CSL)
                            <span class="arrow">▶</span>
                        </div>
                        <div id="setelagoas-courses" class="collapsible-content">
                            <ul class="list-disc list-inside space-y-1">
                                <li>Engenharia Agronômica</li>
                                <li>Engenharia de Alimentos</li>
                                <li>Engenharia Florestal</li>
                                <li>Bacharelado Interdisciplinar em Biosistemas</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="pillars" class="my-16">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-[#C70039]">O Tripé Universitário</h2> <!-- Título vermelho -->
            <p class="text-center text-lg max-w-3xl mx-auto mb-12">A formação na UFSJ é baseada na indissociabilidade entre Ensino, Pesquisa e Extensão, garantindo uma experiência acadêmica completa e cidadã.</p>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-lg text-center">
                    <div class="text-6xl text-gray-800">🎓</div>
                    <h3 class="text-2xl font-bold mt-4">Ensino</h3>
                    <p class="mt-2">Cursos de graduação de alta qualidade, preparando para os desafios do mercado de trabalho e da vida acadêmica. Inclui programas de **Monitoria e Tutoria** para aprimoramento acadêmico.</p>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-lg text-center">
                    <div class="text-6xl text-gray-800">🔬</div>
                    <h3 class="text-2xl font-bold mt-4">Pesquisa</h3>
                    <p class="mt-2">O Programa de Iniciação Científica (PIC) permite aos alunos, sob orientação, contato com grupos de pesquisa e aprendizado de métodos científicos, com **grande número de projetos e bolsas** disponíveis anualmente.</p>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-lg text-center">
                    <div class="text-6xl text-gray-800">🌍</div>
                    <h3 class="text-2xl font-bold mt-4">Extensão</h3>
                    <p class="mt-2">A PROEX conecta a universidade com a comunidade, promovendo **inúmeros projetos e programas de extensão** que contam com a ativa participação de alunos, impactando a sociedade.</p>
                </div>
            </div>
        </section>

        <section id="admissions" class="my-16">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-[#C70039]">Como Ingressar na UFSJ?</h2> <!-- Título vermelho -->
            <p class="text-center text-lg max-w-3xl mx-auto mb-12">O caminho para se tornar um aluno da UFSJ é através do ENEM e do SISU, com um forte compromisso com a inclusão e a diversidade.</p>
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-lg">
                    <h3 class="text-2xl font-bold text-center mb-4">Processo Seletivo via SISU</h3>
                    <div class="space-y-4">
                        <div class="flex items-center">
                            <div class="bg-[#FF5733] text-white rounded-full h-10 w-10 flex items-center justify-center font-bold text-xl">1</div>
                            <p class="ml-4 font-semibold">Realizar o ENEM</p>
                        </div>
                        <div class="h-12 w-px bg-gray-300 ml-5"></div>
                        <div class="flex items-center">
                            <div class="bg-[#FF5733] text-white rounded-full h-10 w-10 flex items-center justify-center font-bold text-xl">2</div>
                            <p class="ml-4 font-semibold">Inscrição no SISU</p>
                        </div>
                         <div class="h-12 w-px bg-gray-300 ml-5"></div>
                        <div class="flex items-center">
                            <div class="bg-[#FF5733] text-white rounded-full h-10 w-10 flex items-center justify-center font-bold text-xl">3</div>
                            <p class="ml-4 font-semibold">Escolher os cursos na UFSJ</p>
                        </div>
                         <div class="h-12 w-px bg-gray-300 ml-5"></div>
                        <div class="flex items-center">
                            <div class="bg-[#FF5733] text-white rounded-full h-10 w-10 flex items-center justify-center font-bold text-xl">4</div>
                            <p class="ml-4 font-semibold">Aguardar o resultado</p>
                        </div>
                    </div>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-lg">
                    <h3 class="text-2xl font-bold text-center mb-4">Ações Afirmativas</h3>
                    <p class="text-lg text-center leading-relaxed">
                        A UFSJ tem um forte compromisso com a inclusão social, reservando 50% de suas vagas para estudantes que cursaram integralmente o ensino fundamental e médio em escolas públicas.
                        Além disso, possui uma ação afirmativa própria, reservando 2% das vagas para pessoas trans.
                        **É fundamental consultar os editais específicos do SISU e da UFSJ para detalhes sobre as diferentes categorias de cotas, que incluem critérios de renda e autodeclaração para pretos, pardos e indígenas, e para ficar atento(a) às documentações necessárias.**
                    </p>
                </div>
            </div>
        </section>

        <section id="campus-life" class="my-16">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-4 text-[#C70039]">Vida no Campus e Oportunidades</h2> <!-- Título vermelho -->
            <p class="text-center text-lg max-w-3xl mx-auto mb-12">A experiência universitária vai muito além da sala de aula, com dezenas de oportunidades para você se desenvolver, competir, empreender e aprimorar sua formação.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">🏆</div>
                    <h3 class="text-xl font-bold mt-3">Atléticas</h3>
                    <p class="mt-1 text-sm">Integração e competições esportivas representando seu curso e a universidade.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">💡</div>
                    <h3 class="text-xl font-bold mt-3">Ligas Acadêmicas</h3>
                    <p class="mt-1 text-sm">Aprofunde seus estudos em temas específicos e desenvolva projetos inovadores.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">🚀</div>
                    <h3 class="text-xl font-bold mt-3">Empresas Juniores</h3>
                    <p class="mt-1 text-sm">Ganhe experiência de mercado, gerenciando projetos reais para clientes.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">⚙️</div>
                    <h3 class="text-xl font-bold mt-3">Equipes de Competição</h3>
                    <p class="mt-1 text-sm">A UFSJ incentiva a participação em equipes de competição de engenharia e tecnologia, como **Baja** (veículos off-road), **Trem que Voa** (aerodesign), e outras. Essas equipes proporcionam experiência prática, trabalho em grupo e a aplicação de conhecimentos em projetos inovadores.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">📚</div>
                    <h3 class="text-xl font-bold mt-3">Programas PET</h3>
                    <p class="mt-1 text-sm">O **Programa de Educação Tutorial (PET)**, presente em diversos cursos como Agronomia, Bioquímica, Filosofia e Mecânica, apoia grupos de excelência em ensino, pesquisa e extensão, oferecendo bolsas e atividades diferenciadas.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">🧑‍🏫</div>
                    <h3 class="text-xl font-bold mt-3">Programas PIBID</h3>
                    <p class="mt-1 text-sm">O **Programa Institucional de Bolsas de Iniciação à Docência (PIBID)** proporciona aos licenciandos uma imersão prática no cotidiano das escolas públicas, com bolsa para formação de futuros professores.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">💰</div>
                    <h3 class="text-xl font-bold mt-3">Pé-de-Meia Licenciaturas</h3>
                    <p class="mt-1 text-sm">Este programa oferece apoio financeiro a estudantes de licenciaturas, com bolsas mensais e incentivo para ingresso na rede pública de ensino, valorizando a carreira docente.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow">
                    <div class="text-5xl">📖</div>
                    <h3 class="text-xl font-bold mt-3">Monitoria e Tutoria</h3>
                    <p class="mt-1 text-sm">Programas que oferecem aos alunos a oportunidade de auxiliar colegas em disciplinas, aprofundando o próprio conhecimento e desenvolvendo habilidades de ensino e liderança.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow lg:col-span-2">
                    <div class="text-5xl">♿</div>
                    <h3 class="text-xl font-bold mt-3">Setor de Inclusão e Acessibilidade (SINAC)</h3>
                    <p class="mt-1 text-sm">O **SINAC** (vinculado à PROAE) promove ações que garantem a inclusão e permanência de pessoas com diversidade funcional (PCDs) no ensino superior. Oferece serviços de tradução/interpretação em Libras, materiais em Braille e apoio pedagógico, buscando um ambiente universitário acolhedor para todos.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg text-center hover:shadow-2xl transition-shadow lg:col-span-2">
                    <div class="text-5xl">🤝</div>
                    <h3 class="text-xl font-bold mt-3">Assistência Estudantil</h3>
                    <p class="mt-1 text-sm">A **Assistência Estudantil**, através da PROAE, oferece suporte essencial para a permanência dos alunos, incluindo acesso a **Restaurantes Universitários (RU)** com refeições acessíveis e, para alguns, **Moradia Estudantil**.</p>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-gray-700 text-white text-center py-16 px-4"> <!-- Fundo cinza escuro -->
        <h2 class="text-3xl md:text-4xl font-black">VENHA PARA A UFSJ!</h2>
        <p class="mt-4 text-lg">Participe da nossa **Mostra de Profissões** em **06 de Outubro**.</p>
        <p class="mt-2 text-lg">Visite nossos campi, conheça os cursos e descubra seu futuro.</p>
        <div class="mt-8">
            <h3 class="text-2xl font-bold mb-4">Assista ao nosso vídeo institucional:</h3>
            <div class="relative w-full max-w-2xl mx-auto" style="padding-top: 56.25%;"> <!-- 16:9 Aspect Ratio -->
                <iframe class="absolute top-0 left-0 w-full h-full rounded-lg shadow-xl" src="https://www.youtube.com/embed/AQc0rMqqA6Y" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </div>
        <a href="https://ufsj.edu.br/" target="_blank" class="mt-8 inline-block bg-[#FF5733] text-white font-bold py-3 px-8 rounded-full hover:bg-[#C70039] transition-colors">Acesse o Site Oficial</a> <!-- Botão laranja/vermelho -->
    </footer>

    <script>
        const tooltipTitleCallback = (tooltipItems) => {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
                return label.join(' ');
            } else {
                return label;
            }
        };
        
        const wrapLabel = (label) => {
            const maxLength = 16;
            if (label.length <= maxLength) return label;
            const words = label.split(' ');
            let lines = [];
            let currentLine = '';
            words.forEach(word => {
                if ((currentLine + word).length > maxLength) {
                    lines.push(currentLine.trim());
                    currentLine = '';
                }
                currentLine += word + ' ';
            });
            lines.push(currentLine.trim());
            return lines;
        };

        const coursesData = {
            labels: ['São João del-Rei', 'Divinópolis', 'Ouro Branco', 'Sete Lagoas'].map(wrapLabel),
            datasets: [{
                label: 'Nº de Cursos',
                data: [23, 4, 5, 4], // Data updated to reflect 4 courses for Sete Lagoas
                backgroundColor: ['#C70039', '#FF5733', '#888888', '#555555'], /* Cores ajustadas para paleta cinza, vermelho e branco */
                borderColor: 'rgba(255, 255, 255, 0.8)',
                borderWidth: 2
            }]
        };

        const coursesCtx = document.getElementById('coursesByCampusChart').getContext('2d');
        new Chart(coursesCtx, {
            type: 'bar',
            data: coursesData,
            options: {
                responsive: true,
                maintainAspectRatio: false,
                indexAxis: 'y',
                scales: {
                    x: {
                        beginAtZero: true,
                        grid: {
                           display: false
                        },
                        ticks: {
                            color: '#4a4a4a' /* Ticks mais escuros para legibilidade no card branco */
                        }
                    },
                    y: {
                        grid: {
                           display: false
                        },
                        ticks: {
                            color: '#4a4a4a' /* Ticks mais escuros para legibilidade no card branco */
                        }
                    }
                },
                plugins: {
                    legend: {
                        display: false
                    },
                    tooltip: {
                        callbacks: {
                           title: tooltipTitleCallback
                        }
                    }
                }
            }
        });

        // Função para alternar seções recolhíveis
        function toggleCollapsible(id) {
            const content = document.getElementById(id);
            const header = content.previousElementSibling;
            if (content.classList.contains('open')) {
                content.classList.remove('open');
                content.style.maxHeight = '0';
                header.classList.remove('active');
            } else {
                // Fecha todas as outras seções abertas
                document.querySelectorAll('.collapsible-content.open').forEach(item => {
                    item.style.maxHeight = '0';
                    item.classList.remove('open');
                    item.previousElementSibling.classList.remove('active');
                });
                // Abre a seção clicada
                content.classList.add('open');
                content.style.maxHeight = content.scrollHeight + 'px'; // Define a altura para a altura do conteúdo
                header.classList.add('active');
            }
        }
    </script>
</body>
</html>
