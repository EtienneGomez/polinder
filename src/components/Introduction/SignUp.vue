<template>
  <div>
    <body class="page page-onboarding preload">
      <main>
        <router-link to="/lobby-one" class="button button-close" role="button"></router-link>

        <section class="row no-gutter reverse-order">
          <div class="col-one-half middle padding">
            <div class="max-width-s">
              <h5>Bienvenidos a Polinder!</h5>
              <p class="paragraph">Introduce tus datos para crear una cuenta.</p>

              <form @submit.prevent="register" enctype="multipart/form-data">
        
              <div class="form-group">
                <label for="nombre">Nombre:</label>
                <input id="nombre" type="text" v-model="nombre" required>
              </div>
              <div class="form-group">
                <label for="apellido">Apellido:</label>
                <input id="apellido" type="text" v-model="apellido" required>
              </div>
              <div class="form-group">
                <label for="boleta">Boleta:</label>
                <input id="boleta" type="text" v-model="boleta" required>
              </div>
              <div class="form-group">
                <label for="correo">Correo:</label>
                <input id="email" type="email" v-model="email" required>
              </div>
              <div class="form-group">
                <label for="contrasena">Contraseña:</label>
                <input id="password" type="password" v-model="password" required>
              </div>
              <div class="form-group">
              <label for="escuelas" class="form-label">Materia que quieres</label>
              <select id="escuelas" class="form-select" v-model="escuela" required>
                <option  selected disabled="selected">Elegir...</option>
                <option selected disabled>////////TURNO VESPERTINO////////</option>
                <option>1CV1	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV1	MATEMATICAS DISCRETAS</option>
                <option>1CV1	CALCULO</option>
                <option>1CV1	ANALISIS VECTORIAL</option>
                <option>1CV1	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV2	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV2	MATEMATICAS DISCRETAS</option>
                <option>1CV2	CALCULO</option>
                <option>1CV2	ANALISIS VECTORIAL</option>
                <option>1CV2	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV3	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV3	MATEMATICAS DISCRETAS</option>
                <option>1CV3	CALCULO</option>
                <option>1CV3	ANALISIS VECTORIAL</option>
                <option>1CV3	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV4	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV4	MATEMATICAS DISCRETAS</option>
                <option>1CV4	CALCULO</option>
                <option>1CV4	ANALISIS VECTORIAL</option>
                <option>1CV4	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV5	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV5	MATEMATICAS DISCRETAS</option>
                <option>1CV5	CALCULO</option>
                <option>1CV5	ANALISIS VECTORIAL</option>
                <option>1CV5	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV6	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV6	MATEMATICAS DISCRETAS</option>
                <option>1CV6	CALCULO</option>
                <option>1CV6	ANALISIS VECTORIAL</option>
                <option>1CV6	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV7	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV7	MATEMATICAS DISCRETAS</option>
                <option>1CV7	CALCULO</option>
                <option>1CV7	ANALISIS VECTORIAL</option>
                <option>1CV7	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV8	CALCULO</option>
                <option>1CV8	ANALISIS VECTORIAL</option>
                <option>2CV1	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV1	ALGEBRA LINEAL</option>
                <option>2CV1	CALCULO APLICADO</option>
                <option>2CV1	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV1	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV1	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV2	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV2	ALGEBRA LINEAL</option>
                <option>2CV2	CALCULO APLICADO</option>
                <option>2CV2	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV2	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV2	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV3	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV3	ALGEBRA LINEAL</option>
                <option>2CV3	CALCULO APLICADO</option>
                <option>2CV3	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV3	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV3	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV4	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV4	ALGEBRA LINEAL</option>
                <option>2CV4	CALCULO APLICADO</option>
                <option>2CV4	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV4	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV4	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV5	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV5	ALGEBRA LINEAL</option>
                <option>2CV5	CALCULO APLICADO</option>
                <option>2CV5	MECANICA Y ELECTROMAGNETISMO</option>
                <option>3CV1	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV1	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV1	ECUACIONES DIFERENCIALES</option>
                <option>3CV1	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV1	CIRCUITOS ELECTRICOS</option>
                <option>3CV1	BASES DE DATOS</option>
                <option>3CV1	FINANZAS EMPRESARIALES</option>
                <option>3CV2	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV2	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV2	ECUACIONES DIFERENCIALES</option>
                <option>3CV2	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV2	CIRCUITOS ELECTRICOS</option>
                <option>3CV2	BASES DE DATOS</option>
                <option>3CV2	FINANZAS EMPRESARIALES</option>
                <option>3CV3	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV3	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV3	ECUACIONES DIFERENCIALES</option>
                <option>3CV3	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV3	CIRCUITOS ELECTRICOS</option>
                <option>3CV3	FINANZAS EMPRESARIALES</option>
                <option>3CV4	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV4	ECUACIONES DIFERENCIALES</option>
                <option>3CV4	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV4	CIRCUITOS ELECTRICOS</option>
                <option>3CV4	BASES DE DATOS</option>
                <option>3CV4	FINANZAS EMPRESARIALES</option>
                <option>3CV5	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV5	ECUACIONES DIFERENCIALES</option>
                <option>3CV5	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV5	CIRCUITOS ELECTRICOS</option>
                <option>3CV5	BASES DE DATOS</option>
                <option>3CV5	FINANZAS EMPRESARIALES</option>
                <option>3CV6	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV6	ECUACIONES DIFERENCIALES</option>
                <option>3CV6	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV6	CIRCUITOS ELECTRICOS</option>
                <option>3CV6	BASES DE DATOS</option>
                <option>3CV6	FINANZAS EMPRESARIALES</option>
                <option>4CV1	TEORIA DE LA COMPUTACION</option>
                <option>4CV1	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV1	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CV1	DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV1	ELECTRONICA ANALOGICA</option>
                <option>4CV1	TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV1	SISTEMAS OPERATIVOS</option>
                <option>4CV2	TEORIA DE LA COMPUTACION</option>
                <option>4CV2	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV2	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CV2	DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV2	ELECTRONICA ANALOGICA</option>
                <option>4CV2	TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV2	SISTEMAS OPERATIVOS</option>
                <option>4CV3	TEORIA DE LA COMPUTACION</option>
                <option>4CV3	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV3	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CV3	DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV3	ELECTRONICA ANALOGICA</option>
                <option>4CV3	TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV3	SISTEMAS OPERATIVOS</option>
                <option>4CV4	TEORIA DE LA COMPUTACION</option>
                <option>4CV4	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV4	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>		 	 
                <option>4CV4 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV4 ELECTRONICA ANALOGICA</option>
                <option>4CV4 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV4 SISTEMAS OPERATIVOS</option>
                <option>5CV1 COMPILADORES</option>
                <option>5CV1 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV1 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV1 INSTRUMENTACION Y CONTROL</option>
                <option>5CV1 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV1 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV1 REDES DE COMPUTADORAS</option>
                <option>5CV2 COMPILADORES</option>
                <option>5CV2 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV2 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV2 INSTRUMENTACION Y CONTROL</option>
                <option>5CV2 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV2 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV2 REDES DE COMPUTADORAS</option>
                <option>5CV3 COMPILADORES</option>
                <option>5CV3 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV3 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV3 INSTRUMENTACION Y CONTROL</option>
                <option>5CV3 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV3 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV3 REDES DE COMPUTADORAS</option>
                <option>5CV4 COMPILADORES</option>
                <option>5CV4 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV4 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV4 INSTRUMENTACION Y CONTROL</option>
                <option>5CV4 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV4 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV4 REDES DE COMPUTADORAS</option>
                <option>6CV1 INTELIGENCIA ARTIFICIAL</option>
                <option>6CV1 SISTEMAS EN CHIP</option>
                <option>6CV1 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CV1 PROC. DE LENG. NAT|MACHINE LEARNING</option>
                <option>6CV1 ALGORITMOS BIOINSPIRADOS|GENETIC ALGORITHMS</option>
                <option>6CV1 INGENIERIA DE SOFTWARE</option>
                <option>6CV1 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CV2 INTELIGENCIA ARTIFICIAL</option>
                <option>6CV2 SISTEMAS EN CHIP</option>
                <option>6CV2 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CV2 INTERNET DE LAS COSAS|EMBEDDED SYSTEMS</option>
                <option>6CV2 COMPUTACION GRAFICA|COMPUTER GRAPHICS</option>
                <option>6CV2 INGENIERIA DE SOFTWARE</option>
                <option>6CV2 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CV3 INTELIGENCIA ARTIFICIAL</option>
                <option>6CV3 SISTEMAS EN CHIP</option>
                <option>6CV3 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CV3 DES. DE APLIC|SOFTWARE QUALLITY ASSURANCE AND DESING PATTERNS</option>
                <option>6CV3 GOBIERNO DE TI|COMPUTER SECURITY</option>
                <option>6CV3 INGENIERIA DE SOFTWARE GONZALEZ RAMIREZ MARKO ALFONSO</option>
                <option>6CV3 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>7CV1 TRABAJO TERMINAL I</option>
                <option>7CV1 SISTEMAS DISTRIBUIDOS</option>
                <option>7CV1 INTERNET DE LAS COSAS|INTERNET OF THINGS</option>
                <option>7CV1 GOBIERNO DE TI|IT GOVERNANCE</option>
                <option>7CV1 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CV2 SISTEMAS DISTRIBUIDOS</option>
                <option>7CV2 COMPUTACION GRAFICA|VIRTUAL AND AUGMENTED REALITY</option>
                <option>7CV2 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CV2 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CV3 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CV10 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CV10 TOPICOS SEL. DE COM|COMPUTTING SELECTED TOPICS II</option>
                <option>8CV1 LIDERAZGO PERSONAL</option>
                <option>8CV1 GESTION EMPRESARIAL</option>
                <option>8CV1 DESARROLLO DE HABILIDADES SOCIALES PARA LA ALTA DIRECCION</option>
                <option selected disabled>////////TURNO MATUTINO////////</option>
                <option>1CM1 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM1 MATEMATICAS DISCRETAS</option>
                <option>1CM1 CALCULO</option>
                <option>1CM1 ANALISIS VECTORIAL</option>
                <option>1CM1 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM2 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM2 MATEMATICAS DISCRETAS</option>
                <option>1CM2 CALCULO</option>
                <option>1CM2 ANALISIS VECTORIAL</option>
                <option>1CM2 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM3 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM3 MATEMATICAS DISCRETAS</option>
                <option>1CM3 CALCULO</option>
                <option>1CM3 ANALISIS VECTORIAL</option>
                <option>1CM3 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM4 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM4 MATEMATICAS DISCRETAS</option>
                <option>1CM4 CALCULO</option>
                <option>1CM4 ANALISIS VECTORIAL</option>
                <option>1CM4 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM5 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM5 MATEMATICAS DISCRETAS</option>
                <option>1CM5 CALCULO</option>
                <option>1CM5 ANALISIS VECTORIAL</option>
                <option>1CM5 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM6 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM6 MATEMATICAS DISCRETAS</option>
                <option>1CM6 CALCULO</option>
                <option>1CM6 ANALISIS VECTORIAL</option>
                <option>1CM6 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM7 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM7 MATEMATICAS DISCRETAS</option>
                <option>1CM7 CALCULO</option>
                <option>1CM7 ANALISIS VECTORIAL</option>
                <option>1CM7 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM8 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM8 MATEMATICAS DISCRETAS</option>
                <option>1CM8 CALCULO</option>
                <option>1CM8 ANALISIS VECTORIAL</option>
                <option>2CM1 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM1 ALGEBRA LINEAL</option>
                <option>2CM1 CALCULO APLICADO</option>
                <option>2CM1 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM1 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM1 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM2 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM2 ALGEBRA LINEAL</option>
                <option>2CM2 CALCULO APLICADO</option>
                <option>2CM2 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM2 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM2 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM3 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM3 ALGEBRA LINEAL</option>
                <option>2CM3 CALCULO APLICADO</option>
                <option>2CM3 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM3 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM3 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM4 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM4 ALGEBRA LINEAL</option>
                <option>2CM4 CALCULO APLICADO</option>
                <option>2CM4 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM4 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM4 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM5 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM5 ALGEBRA LINEAL</option>
                <option>2CM5 CALCULO APLICADO</option>
                <option>2CM5 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM6 CALCULO APLICADO</option>
                <option>3CM1 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM1 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM1 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM1 CIRCUITOS ELECTRICOS</option>
                <option>3CM1 BASES DE DATOS</option>
                <option>3CM1 FINANZAS EMPRESARIALES</option>
                <option>3CM2 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM2 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM2 ECUACIONES DIFERENCIALES</option>
                <option>3CM2 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM2 CIRCUITOS ELECTRICOS</option>
                <option>3CM2 BASES DE DATOS</option>
                <option>3CM2 FINANZAS EMPRESARIALES</option>
                <option>3CM3 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM3 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM3 ECUACIONES DIFERENCIALES</option>
                <option>3CM3 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM3 CIRCUITOS ELECTRICOS</option>
                <option>3CM3 BASES DE DATOS</option>
                <option>3CM3 FINANZAS EMPRESARIALES</option>
                <option>3CM4 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM4 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM4 ECUACIONES DIFERENCIALES</option>
                <option>3CM4 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM4 CIRCUITOS ELECTRICOS</option>
                <option>3CM4 BASES DE DATOS</option>
                <option>3CM4 FINANZAS EMPRESARIALES</option>
                <option>3CM5 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM5 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM5 ECUACIONES DIFERENCIALES</option>
                <option>3CM5 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM5 CIRCUITOS ELECTRICOS</option>
                <option>3CM5 BASES DE DATOS</option>
                <option>3CM5 FINANZAS EMPRESARIALES</option>
                <option>3CM6 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM6 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM6 ECUACIONES DIFERENCIALES</option>
                <option>3CM6 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM6 CIRCUITOS ELECTRICOS</option>
                <option>3CM6 BASES DE DATOS</option>
                <option>3CM6 FINANZAS EMPRESARIALES</option>
                <option>3CM7 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM7 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM7 ECUACIONES DIFERENCIALES</option>
                <option>3CM7 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM7 CIRCUITOS ELECTRICOS</option>
                <option>3CM7 BASES DE DATOS</option>
                <option>4CM1 TEORIA DE LA COMPUTACION</option>
                <option>4CM1 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM1 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM1 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM1 ELECTRONICA ANALOGICA</option>
                <option>4CM1 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM1 SISTEMAS OPERATIVOS</option>
                <option>4CM2 TEORIA DE LA COMPUTACION</option>
                <option>4CM2 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM2 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM2 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM2 ELECTRONICA ANALOGICA</option>
                <option>4CM2 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM2 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM2 SISTEMAS OPERATIVOS</option>
                <option>4CM3 TEORIA DE LA COMPUTACION</option>
                <option>4CM3 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM3 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM3 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM3 ELECTRONICA ANALOGICA</option>
                <option>4CM3 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM3 SISTEMAS OPERATIVOS</option>
                <option>4CM4 TEORIA DE LA COMPUTACION</option>
                <option>4CM4 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM4 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM4 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM4 ELECTRONICA ANALOGICA</option>
                <option>4CM4 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM4 SISTEMAS OPERATIVOS</option>
                <option>4CM5 TEORIA DE LA COMPUTACION</option>
                <option>4CM5 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM5 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM5 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM5 ELECTRONICA ANALOGICA</option>
                <option>4CM5 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM5 SISTEMAS OPERATIVOS</option>
                <option>5CM1 COMPILADORES</option>
                <option>5CM1 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM1 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM1 INSTRUMENTACION Y CONTROL</option>
                <option>5CM1 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM1 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM1 REDES DE COMPUTADORAS</option>
                <option>5CM2 COMPILADORES</option>
                <option>5CM2 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM2 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM2 INSTRUMENTACION Y CONTROL</option>
                <option>5CM2 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM2 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM2 REDES DE COMPUTADORAS</option>
                <option>5CM3 COMPILADORES</option>
                <option>5CM3 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM3 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM3 INSTRUMENTACION Y CONTROL</option>
                <option>5CM3 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM3 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM3 REDES DE COMPUTADORAS</option>
                <option>5CM4 COMPILADORES</option>
                <option>5CM4 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM4 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM4 INSTRUMENTACION Y CONTROL</option>
                <option>5CM4 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM4 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM4 REDES DE COMPUTADORAS</option>
                <option>6CM1 INTELIGENCIA ARTIFICIAL</option>
                <option>6CM1 SISTEMAS EN CHIP</option>
                <option>6CM1 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CM1 BIG DATA|NON-RELATIONAL DATABASES</option>
                <option>6CM1 MINERIA DE DATOS|STATISTICAL TOOLS FOR DATA ANALYTICS</option>
                <option>6CM1 INGENIERIA DE SOFTWARE</option>
                <option>6CM1 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CM2 INTELIGENCIA ARTIFICIAL</option>
                <option>6CM2 SISTEMAS EN CHIP</option>
                <option>6CM2 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CM2 DES. DE APLIC|SOFTWARE QUALLITY ASSURANCE AND DESING PATTERNS</option>
                <option>6CM2 CRIPTOGRAFIA|INTRODUCTION TO CRYPTOGRAPHY</option>
                <option>6CM2 INGENIERIA DE SOFTWARE</option>
                <option>6CM2 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CM3 INTELIGENCIA ARTIFICIAL</option>
                <option>6CM3 SISTEMAS EN CHIP</option>
                <option>6CM3 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CM3 PROC. DE LENG. NAT|MACHINE LEARNING</option>
                <option>6CM3 SISTEMAS COMPLEJOS|CELLULAR AUTOMATA</option>
                <option>6CM3 INGENIERIA DE SOFTWARE</option>
                <option>6CM3 APLICACIONES PARA COMUNICACIONES EN RED MORENO</option>
                <option>6CM10 ALGORITMOS BIOINSPIRADOS|GENETIC ALGORITHMS</option>
                <option>6CM10 TOPICOS SEL. DE COM|COMPUTIG SELECTED TOPICS I</option>
                <option>6CM11 BIG DATA|NON-RELATIONAL DATABASES</option>
                <option>6CM11 GOBIERNO DE TI|COMPUTER SECURITY</option>
                <option>6CM11 CRIPTOGRAFIA|INTRODUCTION TO CRYPTOGRAPHY</option>
                <option>6CM11 VISION POR COMPUTADORA|MACHINE LEARNING</option>
                <option>6CM11 TOPICOS SEL. DE COM|COMPUTTING SELECTED TOPICS I</option>
                <option>7CM1 TRABAJO TERMINAL I</option>
                <option>7CM1 GOBIERNO DE TI|IT GOVERNANCE</option>
                <option>7CM1 CRIPTOGRAFIA|SELECTED TOPICS IN CRYPTOGRAPHY</option>
                <option>7CM1 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CM1 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CM2 SISTEMAS DISTRIBUIDOS</option>
                <option>7CM2 BIG DATA|BIG DATA</option>
                <option>7CM2 DES. DE APLIC|WEB CLIENT AND BACKEND DEVELOPMEN FRAMEWORKS</option>
                <option>7CM2 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CM2 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CM3 SISTEMAS DISTRIBUIDOS</option>
                <option>7CM3 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CM3 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CM10 BIG DATA|BIG DATA</option>
                <option>7CM10 MINERIA DE DATOS|DATA MINING</option>
                <option>7CM10 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CM11 MINERIA DE DATOS|DATA MINING</option>
                <option>7CM11 GOBIERNO DE TI|IT GOVERNANCE</option>
                <option>7CM11 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CM11 VISION POR COMPUTADORA|IMAGE ANALYSIS</option>
                <option>7CM11 TOPICOS SEL. DE COM|COMPUTTING SELECTED TOPICS II</option>
                <option>8CM1 TRABAJO TERMINAL II</option>
                <option>8CM1 LIDERAZGO PERSONAL</option>
                <option>8CM1 GESTION EMPRESARIAL</option>
                <option>8CM1 DESARROLLO DE HABILIDADES SOCIALES PARA LA ALTA DIRECCION</option>
                <option>8CM2 LIDERAZGO PERSONAL</option>
                <option>8CM2 GESTION EMPRESARIAL</option>
                <option>8CM2 DESARROLLO DE HABILIDADES SOCIALES PARA LA ALTA DIRECCION</option> 
              </select>
            </div>
              <div class="form-group">
                <label for="telefono">Telefono:</label>
                <input id="telefono" type="text" v-model="telefono" required>
              </div>
              <div class="form-group">
                <label for="planRelacion">Materia que no quieres:</label>
                <select id="planRelacion" class="form-select" v-model="planRelacion" required>
                <option  selected disabled="selected">Elegir...</option>
                <option selected disabled>////////TURNO VESPERTINO////////</option>
                <option>1CV1	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV1	MATEMATICAS DISCRETAS</option>
                <option>1CV1	CALCULO</option>
                <option>1CV1	ANALISIS VECTORIAL</option>
                <option>1CV1	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV2	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV2	MATEMATICAS DISCRETAS</option>
                <option>1CV2	CALCULO</option>
                <option>1CV2	ANALISIS VECTORIAL</option>
                <option>1CV2	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV3	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV3	MATEMATICAS DISCRETAS</option>
                <option>1CV3	CALCULO</option>
                <option>1CV3	ANALISIS VECTORIAL</option>
                <option>1CV3	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV4	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV4	MATEMATICAS DISCRETAS</option>
                <option>1CV4	CALCULO</option>
                <option>1CV4	ANALISIS VECTORIAL</option>
                <option>1CV4	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV5	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV5	MATEMATICAS DISCRETAS</option>
                <option>1CV5	CALCULO</option>
                <option>1CV5	ANALISIS VECTORIAL</option>
                <option>1CV5	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV6	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV6	MATEMATICAS DISCRETAS</option>
                <option>1CV6	CALCULO</option>
                <option>1CV6	ANALISIS VECTORIAL</option>
                <option>1CV6	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV7	FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CV7	MATEMATICAS DISCRETAS</option>
                <option>1CV7	CALCULO</option>
                <option>1CV7	ANALISIS VECTORIAL</option>
                <option>1CV7	COMUNICACION ORAL Y ESCRITA</option>
                <option>1CV8	CALCULO</option>
                <option>1CV8	ANALISIS VECTORIAL</option>
                <option>2CV1	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV1	ALGEBRA LINEAL</option>
                <option>2CV1	CALCULO APLICADO</option>
                <option>2CV1	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV1	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV1	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV2	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV2	ALGEBRA LINEAL</option>
                <option>2CV2	CALCULO APLICADO</option>
                <option>2CV2	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV2	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV2	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV3	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV3	ALGEBRA LINEAL</option>
                <option>2CV3	CALCULO APLICADO</option>
                <option>2CV3	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV3	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV3	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV4	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV4	ALGEBRA LINEAL</option>
                <option>2CV4	CALCULO APLICADO</option>
                <option>2CV4	MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CV4	INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CV4	FUNDAMENTOS ECONOMICOS</option>
                <option>2CV5	ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CV5	ALGEBRA LINEAL</option>
                <option>2CV5	CALCULO APLICADO</option>
                <option>2CV5	MECANICA Y ELECTROMAGNETISMO</option>
                <option>3CV1	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV1	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV1	ECUACIONES DIFERENCIALES</option>
                <option>3CV1	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV1	CIRCUITOS ELECTRICOS</option>
                <option>3CV1	BASES DE DATOS</option>
                <option>3CV1	FINANZAS EMPRESARIALES</option>
                <option>3CV2	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV2	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV2	ECUACIONES DIFERENCIALES</option>
                <option>3CV2	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV2	CIRCUITOS ELECTRICOS</option>
                <option>3CV2	BASES DE DATOS</option>
                <option>3CV2	FINANZAS EMPRESARIALES</option>
                <option>3CV3	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV3	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV3	ECUACIONES DIFERENCIALES</option>
                <option>3CV3	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV3	CIRCUITOS ELECTRICOS</option>
                <option>3CV3	FINANZAS EMPRESARIALES</option>
                <option>3CV4	ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CV4	ECUACIONES DIFERENCIALES</option>
                <option>3CV4	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV4	CIRCUITOS ELECTRICOS</option>
                <option>3CV4	BASES DE DATOS</option>
                <option>3CV4	FINANZAS EMPRESARIALES</option>
                <option>3CV5	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV5	ECUACIONES DIFERENCIALES</option>
                <option>3CV5	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV5	CIRCUITOS ELECTRICOS</option>
                <option>3CV5	BASES DE DATOS</option>
                <option>3CV5	FINANZAS EMPRESARIALES</option>
                <option>3CV6	PARADIGMAS DE PROGRAMACION</option>
                <option>3CV6	ECUACIONES DIFERENCIALES</option>
                <option>3CV6	FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CV6	CIRCUITOS ELECTRICOS</option>
                <option>3CV6	BASES DE DATOS</option>
                <option>3CV6	FINANZAS EMPRESARIALES</option>
                <option>4CV1	TEORIA DE LA COMPUTACION</option>
                <option>4CV1	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV1	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CV1	DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV1	ELECTRONICA ANALOGICA</option>
                <option>4CV1	TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV1	SISTEMAS OPERATIVOS</option>
                <option>4CV2	TEORIA DE LA COMPUTACION</option>
                <option>4CV2	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV2	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CV2	DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV2	ELECTRONICA ANALOGICA</option>
                <option>4CV2	TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV2	SISTEMAS OPERATIVOS</option>
                <option>4CV3	TEORIA DE LA COMPUTACION</option>
                <option>4CV3	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV3	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CV3	DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV3	ELECTRONICA ANALOGICA</option>
                <option>4CV3	TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV3	SISTEMAS OPERATIVOS</option>
                <option>4CV4	TEORIA DE LA COMPUTACION</option>
                <option>4CV4	PROBABILIDAD Y ESTADISTICA</option>
                <option>4CV4	MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>		 	 
                <option>4CV4 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CV4 ELECTRONICA ANALOGICA</option>
                <option>4CV4 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CV4 SISTEMAS OPERATIVOS</option>
                <option>5CV1 COMPILADORES</option>
                <option>5CV1 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV1 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV1 INSTRUMENTACION Y CONTROL</option>
                <option>5CV1 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV1 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV1 REDES DE COMPUTADORAS</option>
                <option>5CV2 COMPILADORES</option>
                <option>5CV2 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV2 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV2 INSTRUMENTACION Y CONTROL</option>
                <option>5CV2 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV2 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV2 REDES DE COMPUTADORAS</option>
                <option>5CV3 COMPILADORES</option>
                <option>5CV3 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV3 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV3 INSTRUMENTACION Y CONTROL</option>
                <option>5CV3 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV3 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV3 REDES DE COMPUTADORAS</option>
                <option>5CV4 COMPILADORES</option>
                <option>5CV4 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CV4 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CV4 INSTRUMENTACION Y CONTROL</option>
                <option>5CV4 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CV4 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CV4 REDES DE COMPUTADORAS</option>
                <option>6CV1 INTELIGENCIA ARTIFICIAL</option>
                <option>6CV1 SISTEMAS EN CHIP</option>
                <option>6CV1 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CV1 PROC. DE LENG. NAT|MACHINE LEARNING</option>
                <option>6CV1 ALGORITMOS BIOINSPIRADOS|GENETIC ALGORITHMS</option>
                <option>6CV1 INGENIERIA DE SOFTWARE</option>
                <option>6CV1 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CV2 INTELIGENCIA ARTIFICIAL</option>
                <option>6CV2 SISTEMAS EN CHIP</option>
                <option>6CV2 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CV2 INTERNET DE LAS COSAS|EMBEDDED SYSTEMS</option>
                <option>6CV2 COMPUTACION GRAFICA|COMPUTER GRAPHICS</option>
                <option>6CV2 INGENIERIA DE SOFTWARE</option>
                <option>6CV2 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CV3 INTELIGENCIA ARTIFICIAL</option>
                <option>6CV3 SISTEMAS EN CHIP</option>
                <option>6CV3 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CV3 DES. DE APLIC|SOFTWARE QUALLITY ASSURANCE AND DESING PATTERNS</option>
                <option>6CV3 GOBIERNO DE TI|COMPUTER SECURITY</option>
                <option>6CV3 INGENIERIA DE SOFTWARE GONZALEZ RAMIREZ MARKO ALFONSO</option>
                <option>6CV3 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>7CV1 TRABAJO TERMINAL I</option>
                <option>7CV1 SISTEMAS DISTRIBUIDOS</option>
                <option>7CV1 INTERNET DE LAS COSAS|INTERNET OF THINGS</option>
                <option>7CV1 GOBIERNO DE TI|IT GOVERNANCE</option>
                <option>7CV1 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CV2 SISTEMAS DISTRIBUIDOS</option>
                <option>7CV2 COMPUTACION GRAFICA|VIRTUAL AND AUGMENTED REALITY</option>
                <option>7CV2 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CV2 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CV3 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CV10 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CV10 TOPICOS SEL. DE COM|COMPUTTING SELECTED TOPICS II</option>
                <option>8CV1 LIDERAZGO PERSONAL</option>
                <option>8CV1 GESTION EMPRESARIAL</option>
                <option>8CV1 DESARROLLO DE HABILIDADES SOCIALES PARA LA ALTA DIRECCION</option>
                <option selected disabled>////////TURNO MATUTINO////////</option>
                <option>1CM1 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM1 MATEMATICAS DISCRETAS</option>
                <option>1CM1 CALCULO</option>
                <option>1CM1 ANALISIS VECTORIAL</option>
                <option>1CM1 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM2 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM2 MATEMATICAS DISCRETAS</option>
                <option>1CM2 CALCULO</option>
                <option>1CM2 ANALISIS VECTORIAL</option>
                <option>1CM2 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM3 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM3 MATEMATICAS DISCRETAS</option>
                <option>1CM3 CALCULO</option>
                <option>1CM3 ANALISIS VECTORIAL</option>
                <option>1CM3 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM4 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM4 MATEMATICAS DISCRETAS</option>
                <option>1CM4 CALCULO</option>
                <option>1CM4 ANALISIS VECTORIAL</option>
                <option>1CM4 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM5 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM5 MATEMATICAS DISCRETAS</option>
                <option>1CM5 CALCULO</option>
                <option>1CM5 ANALISIS VECTORIAL</option>
                <option>1CM5 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM6 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM6 MATEMATICAS DISCRETAS</option>
                <option>1CM6 CALCULO</option>
                <option>1CM6 ANALISIS VECTORIAL</option>
                <option>1CM6 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM7 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM7 MATEMATICAS DISCRETAS</option>
                <option>1CM7 CALCULO</option>
                <option>1CM7 ANALISIS VECTORIAL</option>
                <option>1CM7 COMUNICACION ORAL Y ESCRITA</option>
                <option>1CM8 FUNDAMENTOS DE PROGRAMACION</option>
                <option>1CM8 MATEMATICAS DISCRETAS</option>
                <option>1CM8 CALCULO</option>
                <option>1CM8 ANALISIS VECTORIAL</option>
                <option>2CM1 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM1 ALGEBRA LINEAL</option>
                <option>2CM1 CALCULO APLICADO</option>
                <option>2CM1 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM1 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM1 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM2 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM2 ALGEBRA LINEAL</option>
                <option>2CM2 CALCULO APLICADO</option>
                <option>2CM2 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM2 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM2 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM3 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM3 ALGEBRA LINEAL</option>
                <option>2CM3 CALCULO APLICADO</option>
                <option>2CM3 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM3 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM3 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM4 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM4 ALGEBRA LINEAL</option>
                <option>2CM4 CALCULO APLICADO</option>
                <option>2CM4 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM4 INGENIERIA ETICA Y SOCIEDAD</option>
                <option>2CM4 FUNDAMENTOS ECONOMICOS</option>
                <option>2CM5 ALGORITMOS Y ESTRUCTURA DE DATOS</option>
                <option>2CM5 ALGEBRA LINEAL</option>
                <option>2CM5 CALCULO APLICADO</option>
                <option>2CM5 MECANICA Y ELECTROMAGNETISMO</option>
                <option>2CM6 CALCULO APLICADO</option>
                <option>3CM1 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM1 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM1 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM1 CIRCUITOS ELECTRICOS</option>
                <option>3CM1 BASES DE DATOS</option>
                <option>3CM1 FINANZAS EMPRESARIALES</option>
                <option>3CM2 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM2 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM2 ECUACIONES DIFERENCIALES</option>
                <option>3CM2 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM2 CIRCUITOS ELECTRICOS</option>
                <option>3CM2 BASES DE DATOS</option>
                <option>3CM2 FINANZAS EMPRESARIALES</option>
                <option>3CM3 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM3 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM3 ECUACIONES DIFERENCIALES</option>
                <option>3CM3 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM3 CIRCUITOS ELECTRICOS</option>
                <option>3CM3 BASES DE DATOS</option>
                <option>3CM3 FINANZAS EMPRESARIALES</option>
                <option>3CM4 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM4 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM4 ECUACIONES DIFERENCIALES</option>
                <option>3CM4 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM4 CIRCUITOS ELECTRICOS</option>
                <option>3CM4 BASES DE DATOS</option>
                <option>3CM4 FINANZAS EMPRESARIALES</option>
                <option>3CM5 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM5 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM5 ECUACIONES DIFERENCIALES</option>
                <option>3CM5 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM5 CIRCUITOS ELECTRICOS</option>
                <option>3CM5 BASES DE DATOS</option>
                <option>3CM5 FINANZAS EMPRESARIALES</option>
                <option>3CM6 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM6 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM6 ECUACIONES DIFERENCIALES</option>
                <option>3CM6 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM6 CIRCUITOS ELECTRICOS</option>
                <option>3CM6 BASES DE DATOS</option>
                <option>3CM6 FINANZAS EMPRESARIALES</option>
                <option>3CM7 ANALISIS Y DISEÑO DE ALGORITMOS</option>
                <option>3CM7 PARADIGMAS DE PROGRAMACION</option>
                <option>3CM7 ECUACIONES DIFERENCIALES</option>
                <option>3CM7 FUNDAMENTOS DE DISEÑO DIGITAL</option>
                <option>3CM7 CIRCUITOS ELECTRICOS</option>
                <option>3CM7 BASES DE DATOS</option>
                <option>4CM1 TEORIA DE LA COMPUTACION</option>
                <option>4CM1 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM1 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM1 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM1 ELECTRONICA ANALOGICA</option>
                <option>4CM1 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM1 SISTEMAS OPERATIVOS</option>
                <option>4CM2 TEORIA DE LA COMPUTACION</option>
                <option>4CM2 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM2 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM2 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM2 ELECTRONICA ANALOGICA</option>
                <option>4CM2 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM2 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM2 SISTEMAS OPERATIVOS</option>
                <option>4CM3 TEORIA DE LA COMPUTACION</option>
                <option>4CM3 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM3 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM3 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM3 ELECTRONICA ANALOGICA</option>
                <option>4CM3 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM3 SISTEMAS OPERATIVOS</option>
                <option>4CM4 TEORIA DE LA COMPUTACION</option>
                <option>4CM4 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM4 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM4 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM4 ELECTRONICA ANALOGICA</option>
                <option>4CM4 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM4 SISTEMAS OPERATIVOS</option>
                <option>4CM5 TEORIA DE LA COMPUTACION</option>
                <option>4CM5 PROBABILIDAD Y ESTADISTICA</option>
                <option>4CM5 MATEMATICAS AVANZADAS PARA LA INGENIERIA</option>
                <option>4CM5 DISEÑO DE SISTEMAS DIGITALES</option>
                <option>4CM5 ELECTRONICA ANALOGICA</option>
                <option>4CM5 TECNOLOGIAS PARA DESARROLLO DE APLICACIONES WEB</option>
                <option>4CM5 SISTEMAS OPERATIVOS</option>
                <option>5CM1 COMPILADORES</option>
                <option>5CM1 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM1 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM1 INSTRUMENTACION Y CONTROL</option>
                <option>5CM1 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM1 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM1 REDES DE COMPUTADORAS</option>
                <option>5CM2 COMPILADORES</option>
                <option>5CM2 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM2 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM2 INSTRUMENTACION Y CONTROL</option>
                <option>5CM2 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM2 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM2 REDES DE COMPUTADORAS</option>
                <option>5CM3 COMPILADORES</option>
                <option>5CM3 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM3 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM3 INSTRUMENTACION Y CONTROL</option>
                <option>5CM3 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM3 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM3 REDES DE COMPUTADORAS</option>
                <option>5CM4 COMPILADORES</option>
                <option>5CM4 PROCESAMIENTO DIGITAL DE SEÑALES</option>
                <option>5CM4 ARQUITECTURA DE COMPUTADORAS</option>
                <option>5CM4 INSTRUMENTACION Y CONTROL</option>
                <option>5CM4 ANALISIS Y DISEÑO DE SISTEMAS</option>
                <option>5CM4 FORMULACION Y EVALUACION DE PROYECTOS INFORMATICOS</option>
                <option>5CM4 REDES DE COMPUTADORAS</option>
                <option>6CM1 INTELIGENCIA ARTIFICIAL</option>
                <option>6CM1 SISTEMAS EN CHIP</option>
                <option>6CM1 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CM1 BIG DATA|NON-RELATIONAL DATABASES</option>
                <option>6CM1 MINERIA DE DATOS|STATISTICAL TOOLS FOR DATA ANALYTICS</option>
                <option>6CM1 INGENIERIA DE SOFTWARE</option>
                <option>6CM1 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CM2 INTELIGENCIA ARTIFICIAL</option>
                <option>6CM2 SISTEMAS EN CHIP</option>
                <option>6CM2 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CM2 DES. DE APLIC|SOFTWARE QUALLITY ASSURANCE AND DESING PATTERNS</option>
                <option>6CM2 CRIPTOGRAFIA|INTRODUCTION TO CRYPTOGRAPHY</option>
                <option>6CM2 INGENIERIA DE SOFTWARE</option>
                <option>6CM2 APLICACIONES PARA COMUNICACIONES EN RED</option>
                <option>6CM3 INTELIGENCIA ARTIFICIAL</option>
                <option>6CM3 SISTEMAS EN CHIP</option>
                <option>6CM3 METODOS CUANTITATIVOS PARA LA TOMA DE DECISIONES</option>
                <option>6CM3 PROC. DE LENG. NAT|MACHINE LEARNING</option>
                <option>6CM3 SISTEMAS COMPLEJOS|CELLULAR AUTOMATA</option>
                <option>6CM3 INGENIERIA DE SOFTWARE</option>
                <option>6CM3 APLICACIONES PARA COMUNICACIONES EN RED MORENO</option>
                <option>6CM10 ALGORITMOS BIOINSPIRADOS|GENETIC ALGORITHMS</option>
                <option>6CM10 TOPICOS SEL. DE COM|COMPUTIG SELECTED TOPICS I</option>
                <option>6CM11 BIG DATA|NON-RELATIONAL DATABASES</option>
                <option>6CM11 GOBIERNO DE TI|COMPUTER SECURITY</option>
                <option>6CM11 CRIPTOGRAFIA|INTRODUCTION TO CRYPTOGRAPHY</option>
                <option>6CM11 VISION POR COMPUTADORA|MACHINE LEARNING</option>
                <option>6CM11 TOPICOS SEL. DE COM|COMPUTTING SELECTED TOPICS I</option>
                <option>7CM1 TRABAJO TERMINAL I</option>
                <option>7CM1 GOBIERNO DE TI|IT GOVERNANCE</option>
                <option>7CM1 CRIPTOGRAFIA|SELECTED TOPICS IN CRYPTOGRAPHY</option>
                <option>7CM1 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CM1 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CM2 SISTEMAS DISTRIBUIDOS</option>
                <option>7CM2 BIG DATA|BIG DATA</option>
                <option>7CM2 DES. DE APLIC|WEB CLIENT AND BACKEND DEVELOPMEN FRAMEWORKS</option>
                <option>7CM2 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CM2 ADMINISTRACION DE SERVICIOS EN RED</option>
                <option>7CM3 SISTEMAS DISTRIBUIDOS</option>
                <option>7CM3 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CM3 DESARROLLO DE APLICACIONES MOVILES NATIVAS</option>
                <option>7CM10 BIG DATA|BIG DATA</option>
                <option>7CM10 MINERIA DE DATOS|DATA MINING</option>
                <option>7CM10 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CM11 MINERIA DE DATOS|DATA MINING</option>
                <option>7CM11 GOBIERNO DE TI|IT GOVERNANCE</option>
                <option>7CM11 PROC. DE LENG|NATURAL LANGUAGE PROCESSING</option>
                <option>7CM11 VISION POR COMPUTADORA|IMAGE ANALYSIS</option>
                <option>7CM11 TOPICOS SEL. DE COM|COMPUTTING SELECTED TOPICS II</option>
                <option>8CM1 TRABAJO TERMINAL II</option>
                <option>8CM1 LIDERAZGO PERSONAL</option>
                <option>8CM1 GESTION EMPRESARIAL</option>
                <option>8CM1 DESARROLLO DE HABILIDADES SOCIALES PARA LA ALTA DIRECCION</option>
                <option>8CM2 LIDERAZGO PERSONAL</option>
                <option>8CM2 GESTION EMPRESARIAL</option>
                <option>8CM2 DESARROLLO DE HABILIDADES SOCIALES PARA LA ALTA DIRECCION</option>
                </select>
              </div>
              <div class="form-group">
                <label for="descripcion">Descripcion:</label>
                <textarea id="description" type="text-area" v-model="descripcion" required> </textarea>
              </div>
              <div class="form-group">
                <label for="imagen">Selecciona tu foto:</label>
                <input type="file" id="imagen" name="imagen" ref="fileInput">
              </div>
              <button type="submit" class="button button-primary full-width space-top">Crear una cuenta</button>
            </form>

            </div>
            <div class="center max-width-s space-top">
              <span class="muted">Al crear una cuenta, acepta nuestros </span><a href="terminos.html">Términos</a><span class="muted">.</span>
            </div>
            <div class="center max-width-s">
              <span class="muted">¿Ya tienes una cuenta? </span><router-link to="/login-page">Iniciar sesión</router-link>
            </div>
          </div>
          <div class="error-dialog" v-if="showErrorEmail">
            <p class="error-message">Error al crear la cuenta. Por favor, asegúrese de ingresar su correo institucional.</p>
          </div>
          <div class="col-one-half bg-image-05 featured-image"></div>
        </section>
      </main>
    </body>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  name: "SignUp",
  data() {
    return {
      showErrorEmail: false,
      imagen: null,
      nombre: "",
      password: "",
      boleta: "",
      escuela: "",
      telefono: "",
      planRelacion: "",
      descripcion: "",
      email: "",
    };
  },
  methods: {


    
    register() {
      const fileInput = this.$refs.fileInput;
      const file = fileInput.files[0];

      const maxSize = 5 * 1024 * 1024; // 5 MB
      if (file.size > maxSize) {
        console.error("El tamaño del archivo excede el límite permitido");
        return;
      }
      var bodyFormData = new FormData();
      bodyFormData.append('email', this.email);
      bodyFormData.append('password', this.password);
      bodyFormData.append('nombre', this.nombre);
      bodyFormData.append('apellido', this.apellido);
      bodyFormData.append('boleta', this.boleta);
      bodyFormData.append('telefono', this.telefono);
      bodyFormData.append('escuela', this.escuela);
      bodyFormData.append('planRelacion', this.planRelacion);
      bodyFormData.append('descripcion', this.descripcion);
      bodyFormData.append('imagen', this.descripcion);

      // Validar el correo electrónico
      if (!this.email.endsWith("@ipn.mx")) {
        // Mostrar mensaje de error o tomar la acción correspondiente
        this.showErrorEmail = true;
        console.error("El correo electrónico debe tener la terminación '@ipn.mx'");
        return;
      }

      // Realizar la solicitud HTTP utilizando Axios
      axios({
        method: "post",
        url: "http://3.144.13.162/registro.php",
        data: bodyFormData,
        headers: { "Content-Type": "multipart/form-data" },
      })
      .then(response => {
        console.log(response.data);
        // Redireccionar a "/login=page"
        this.$router.push("/login-page");
    })
        .catch(error => {
          this.showErrorEmail = false;
          console.log(error);
    });

    },
  },
};

</script>   

<style scoped>
.error-dialog {
  position: fixed;
  top: 60%;
  left: 30%;
  transform: translate(-50%, -50%);
  background-color: #fff;
  border: 1px solid #ccc;
  padding: 20px;
  z-index: 9999;
}

.error-message {
  color: red;
  margin: 0;
}
</style>