---
title: 什么？用自行车也能环游世界？！
date: 2022-12-20
excerpt_separator: "<!--more-->"
categories: 
  - SVG制作
tags:
  - svg

---

#### 大小不同的自行车因地心引力的作用下环绕着地球的<a href="http://animpen.com/pen/2sXIni">SVG动画</a>,试着将鼠标放在小自行车上看看吧！
<!--more-->

通过对原动画添加css过渡的hover，以及使用关键字动画进行设置，运用svg旋转和变换大小两种动画，来实现大小自行车都能一起环游世界的动画效果。

#### 试着将鼠标轻放到小自行车上，小自行车也跟着大自行车一起环游世界啦！
小自行车紧跟其后，就像大小自行车你追我赶一样

<style>
body {
	margin: 0;
	background: skyblue;
}

svg {
	width: 100vw;
}

.Bicicletas {
	display: flex;
	height: 100vh;
	width: 100vw;
	align-items: center;
	justify-content: center;
}

.Rayo {
	fill: none;
	stroke: #666;
	stroke-width: 1;
	stroke-linecap: round;
}

.Metal {
	fill: #666;
}

.Llanta {
	fill: none;
	stroke: #000;
	stroke-width: 14;
	stroke-linecap: round;
}

.Rin {
	fill: none;
	stroke: #666;
	stroke-width: 8;
	stroke-linecap: round;
}

.PalaPedal {
	fill: none;
	stroke: #999;
	stroke-width: 7;
	stroke-linecap: round;
}

.Pedal {
	fill: none;
	stroke: #000;
	stroke-width: 7;
}

.Tacos {
	fill: none;
	stroke: #000;
	stroke-width: 18;
	stroke-dasharray: 11.22;
}

.Cuadro {
	fill: none;
	stroke: purple;
}

.CuadroI {
	fill: none;
	stroke: #FC0;
}

.CuadroII {
	fill: none;
	stroke: green;
}

.Componentes {
	fill: none;
	stroke: black;
	stroke-linejoin: round;
}

.Pedaleo {
	animation: Girando 3s infinite linear;
	transform-origin: 354px 359px
}

.PedalD {
	animation: GirandoBack 3s infinite linear;
	transform-origin: 354px 409px
}

.PedalI {
	animation: GirandoBack 3s infinite linear;
	transform-origin: 354px 309px
}

@keyframes GirandoBack {
	to {
		transform: rotate(-360deg);
	}
}

.Estrellita {
	transform-origin: 198px 401px;
	animation: Girando 2s infinite linear;
}

.Rodando {
	animation: Girando 4s infinite linear;
}

.Delantera {
	transform-origin: 585.71px 354.18px;
}

.Trasera {
	transform-origin: 214.28px 354.18px;
}

@keyframes Girando {
	to {
		transform: rotate(360deg);
	}
}

#Cadena {
	fill: none;
}

.CadenaA {
	stroke: #333;
	stroke-width: 4px;
	stroke-dasharray: 0px 4px;
	stroke-linecap: round;
	animation: CorreCadena 0.5s infinite linear;
}

.CadenaB {
	stroke: #333;
	stroke-width: 3px;
	stroke-dasharray: 4px 4px;
	stroke-linecap: round;
}

.CadenaC {
	stroke: #666;
	stroke-width: 2px;
	stroke-dasharray: 0px 4px;
	stroke-linecap: round;
	animation: CorreCadena 1s infinite linear;
}

@keyframes CorreCadena {
	to {
		stroke-dasharray: 4px 4px;
	}
}

.Dientes {
	stroke-width: 5px;
	stroke-dasharray: 1.5px;
}



.PrimerPlano {
	transform: rotate(-77deg);
	animation: Rodada 6s infinite ease;
	transform-origin: 400px 1000px;
}

@keyframes Rodada {
	to {
		transform: rotate(67deg);
	}
}

#Terreno {
	stroke: #FC0;
	stroke-width: 6px;
	stroke-dasharray: 0px 9.17px;
	stroke-linecap: round;
	animation: Recorrido 2s infinite linear;
	transform-origin: 400px 1000px;
}



@keyframes Recorrido {
	to {
		transform: rotate(-15deg);
	}
}

.SegundoPlano {
	transition: width 1s linear 2s;
	    /* Safari */
	    -webkit-transition:width 1s linear 2s;
}

.SegundoPlano:hover {
	transform: rotate(-57deg);
	animation: Rodadaaa 12s infinite linear;
	transform-origin: 400px 1000px;
	
}

@keyframes Rodadaaa {
	to {
		transform: rotate(57deg);
	}
}

.Cielo {
	animation: Paisaje 30s infinite linear;
	transform-origin: 400px 1000px;
	
}

.Lejania {
	animation: Paisaje 60s infinite linear;
	transform-origin: 400px 1000px;
}

.Cactuses {
	animation: Paisaje 20s infinite linear;
	transform-origin: 400px 1000px;
}

@keyframes Paisaje {
	to {
		transform: rotate(-90deg);
	}
}

</style>

<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
			viewBox="0 0 800 600" style="display: none;">
			<symbol id="Cuadro" viewBox="0 0 800 600">
				<polyline points="323.2,241.7 217.3,354.2 354.5,354.2 318.8,225.8 " stroke-linejoin="round"
					stroke-width="11" />
				<polyline points="519.6,213.3 506,177.9 323.2,241.7 " stroke-width="16" />
				<line x1="354.5" y1="354.2" x2="509" y2="185.7" stroke-width="16" />
			</symbol>
			<path id="Cadena"
				d="M208,369.2c-5.9-2.5-10-8.3-10-15c0-9,7.3-16.3,16.3-16.3l139.2-1c11.9,0,21.5,9.6,21.5,21.5c0,10.5-7.5,19.2-17.5,21.1 l-158.1,29.3c-4.1,0.8-8.8-2.2-8.8-7.3c0-3,1.8-5.7,4.4-6.8l13.5-6.6C216.4,384.1,216.1,372.6,208,369.2z" />
		</svg>
		<!-- Visible -->
		<div class="Bicicletas">
			<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
				viewBox="0 0 800 600">
				<defs>
					<g id="RuedaBike">
						<line id="Valvula" x1="150" y1="50" x2="150" y2="75" stroke="#333" stroke-width="4" />
						<g id="Rayos" class="Rayo">
							<line x1="150" y1="145" x2="50" y2="140" />
							<line x1="150" y1="155" x2="50" y2="160" />
							<line x1="150" y1="145" x2="60" y2="115" />
							<line x1="150" y1="155" x2="60" y2="185" />
						</g>
						<use xlink:href="#Rayos" transform="rotate(60, 150, 150)" />
						<use xlink:href="#Rayos" transform="rotate(120, 150, 150)" />
						<use xlink:href="#Rayos" transform="rotate(180, 150, 150)" />
						<use xlink:href="#Rayos" transform="rotate(240, 150, 150)" />
						<use xlink:href="#Rayos" transform="rotate(300, 150, 150)" />
						<g id="Neumatico">
							<circle cx="150" cy="150" r="100" class="Llanta" />
							<circle cx="150" cy="150" r="100" class="Tacos" />
							<circle cx="150" cy="150" r="90" class="Rin" />
							<g id="Eje">
								<circle cx="150" cy="150" r="15" fill="#999" />
								<circle cx="150" cy="150" r="5" />
							</g>
						</g>
					</g>
					<g id="Bici">
						<g id="Estrella">
							<line id="Gajo" x1="350" y1="350" x2="370" y2="350" fill="none" />
							<use xlink:href="#Gajo" transform="rotate(60, 354, 359)" />
							<use xlink:href="#Gajo" transform="rotate(120, 354, 359)" />
							<use xlink:href="#Gajo" transform="rotate(180, 354, 359)" />
							<use xlink:href="#Gajo" transform="rotate(240, 354, 359)" />
							<use xlink:href="#Gajo" transform="rotate(300, 354, 359)" />
							<circle cx="354" cy="359" r="18.5" fill="none" />
						</g>
						<g id="RuedaTrasera">
							<use xlink:href="#RuedaBike" width="300" height="300" x="64.28" y="204" />
							<circle cx="214.28" cy="354" r="25" class="Dientes" stroke="#666" fill="#666" />
							<circle cx="214.28" cy="354" r="21" class="Dientes" stroke="#999" fill="#999" />
							<circle cx="214.28" cy="354" r="17" class="Dientes" stroke="#666" fill="#666" />
						</g>
						<g id="RuedaDelantera">
							<use xlink:href="#RuedaBike" width="300" height="300" x="435.7" y="204" />
							<use xlink:href="#Estrella" x="114.5" y="-75.5" transform="scale(1.25)" stroke="#999"
								stroke-width="3.5" />
						</g>
						<g id="EstrellaCompleta">
							<use xlink:href="#Estrella" stroke="#666" stroke-width="4" />
							<circle cx="354" cy="359" r="20" class="Dientes" stroke="#666" fill="none" />
							<circle cx="354" cy="359" r="8" />
						</g>
						<g id="gAnterior">
							<g class="Componentes">
								<g id="Cables" stroke-width="2">
									<path d="M548,257c0-24,1-93-40-108" />
									<path d="M514,151c21-2.8,25,14-6,42" />
									<path d="M509,195c18-8,37.8-34,7-43" />
								</g>
								<polygon id="Asiento" points="337.7,141.5 254.7,141.5 280,151.2 " stroke-width="7"
									fill="black" />
								<line id="EspigaAsiento" x1="318.8" y1="225.8" x2="297.2" y2="148.1" stroke-width="7" />
								<polyline id="Manillar" points="504.1,174.1 498.3,159 520.3,145.8 499.1,137 "
									stroke-width="13" stroke-linecap="round" />
								<line id="Tijera" x1="580.9" y1="359" x2="524.5" y2="211.4" stroke-width="13" />
							</g>
						</g>
						<use xlink:href="#Cuadro" class="CuadroI" />
						<g id="Pinion">
							<circle cx="214.28" cy="354" r="13" class="Dientes" stroke="#999" fill="#999" />
							<circle cx="214.28" cy="354" r="9" class="Dientes" stroke="#666" fill="#666" />
							<circle cx="214.28" cy="354" r="5" class="Dientes" stroke="#999" fill="#999" />
						</g>
						<g id="Tirantes">
							<polyline class="CuadroI" points="323.2,241.7 217.3,354.2 289.7,354.2 " stroke-width="11"
								stroke-linejoin="round" />
							<polyline class="Componentes" points="198,401 223,387 201,367 217,354 " stroke-width="6"
								stroke-linecap="round" />
						</g>
					</g>
				</defs>
				<g class="Lejania">
					<path id="Montanias" fill="orange" opacity="0.5"
						d="M-69.7,530.3c8.3-8.3,25.8-7.9,34.3-15.6c8.7-7.8,16.6-17.3,25.6-24.5c9.1-7.3,22.5-9.6,31.9-16.4 c9.5-6.8,36.8,13.9,46.6,7.7c9.8-6.3,17.5-13.3,27.5-19c10.1-5.7,11.7-25.6,22.1-30.7c10.4-5.2,19.3-12.8,29.9-17.4 c10.7-4.6,28.3,10.6,39.2,6.6c10.9-4,11.4-37.3,22.4-40.7c11.1-3.4,30.4,24.8,41.6,22c11.3-2.8,21.1-5.6,32.5-7.8 c11.4-2.2,19.4-19.2,30.9-20.8c11.5-1.6,22.1-7.9,33.6-8.9c11.6-0.9,22.3-22.9,33.9-23.2c11.6-0.3,24,1.8,35.6,2.1 c11.6,0.3,21.8,27.7,33.3,28.6c11.6,0.9,20.8,14.3,32.3,15.8c11.5,1.6,27.2-26.2,38.6-24c11.4,2.2,22.2,7.9,33.5,10.6 c11.3,2.8,14,33.6,25.1,37c11.1,3.4,34.7-31.7,45.6-27.7c10.9,4,23.9,5,34.6,9.6c10.6,4.6,12.1,29.9,22.5,35 c10.4,5.1,28.8-4.4,38.9,1.3c10.1,5.7,3.8,38.1,13.6,44.4c9.7,6.2,24.9,3.3,34.3,10.1c9.4,6.8,9.7,24.1,18.8,31.4 c9,7.2,27.1,2.7,35.8,10.5c8.6,7.7,36.6-4.4,44.9,3.8L400,1000L-69.7,530.3z" />
					<use xlink:href="#Montanias" transform="rotate(90, 400, 1000)" />
				</g>
				<g class="Cielo">
					<g id="Nube" fill="none" stroke="#FFF" stroke-linecap="round">
						<path d="M129.6,212.3c206-70.5,434.2-58,632.4,37.6" stroke-width="50" />
						<path d="M242,211.8c59.1-11.8,119.2-16.9,179.2-15.3" stroke-width="50" />
						<path d="M620.3,124.6c22.6,5.7,45.1,12.2,67.3,19.7" stroke-width="40" />
						<path d="M292.7,104.3c43.5-5.2,87.3-7.2,131-6.1" stroke-width="80" />
						<path d="M183.4,150.3c107.6-27.3,219.5-33.9,329.1-19.8" stroke-width="80" />
						<path d="M1025.3,363.5c20.6,20.2,40.1,41.4,58.6,63.5" stroke-width="70" />
						<path d="M930.6,315.7c60.9,47.3,115.3,102.5,161.6,164.1" stroke-width="40" />
					</g>
					<use xlink:href="#Nube" transform="rotate(90, 400, 1000)" />
				</g>
				<g class="Cactuses">
					<g id="Cactus" fill="none" stroke="#066" stroke-linecap="round">
						<line x1="780.3" y1="600.8" x2="940.3" y2="440.8" stroke-width="16" />
						<line x1="797.1" y1="617.6" x2="900.7" y2="514.1" stroke-width="16" />
						<path d="M858.9,514.1c-8.5-8.5-8.5-22.3,0-30.8l36.4-36.4" stroke-width="14" />
						<path d="M853.7,566.5c8.5,8.5,22.3,8.5,30.8,0l18.8-18.8" stroke-width="14" />
					</g>
					<use xlink:href="#Cactus" transform="rotate(90, 400, 1000)" />
				</g>
				<g class="SegundoPlano">
					<g id="SegundaBici" transform="scale(0.5) translate(400 422)">
						<use xlink:href="#RuedaDelantera" class="Rodando Delantera" />
						<g class="Pedaleo">
							<line class="Pedal PedalI" x1="344" y1="309" x2="364" y2="309" />
							<line class="PalaPedal" x1="354" y1="309" x2="354" y2="359" />
						</g>
						<use xlink:href="#gAnterior" />
						<use xlink:href="#RuedaTrasera" class="Rodando Trasera" />
						<use xlink:href="#Cuadro" class="Cuadro" />
						<use xlink:href="#EstrellaCompleta" class="Pedaleo" />
						<circle class="Estrellita Dientes" cx="198" cy="401" r="6" stroke="#999" fill="#999" />
						<use xlink:href="#Cadena" class="CadenaA" />
						<use xlink:href="#Cadena" class="CadenaB" />
						<use xlink:href="#Cadena" class="CadenaC" />
						<use xlink:href="#Pinion" class="Rodando Trasera" />
						<polyline class="Cuadro" points="323.2,241.7 217.3,354.2 289.7,354.2 " stroke-width="11"
							stroke-linejoin="round" />
						<polyline class="Componentes" points="198,401 223,387 201,367 217,354 " stroke-width="6"
							stroke-linecap="round" />
						<g class="Pedaleo">
							<line class="PalaPedal" x1="354" y1="359" x2="354" y2="409" />
							<line class="Pedal PedalD" x1="344" y1="409" x2="364" y2="409" />
						</g>
					</g>
				</g>
				<circle id="Camino" cx="400" cy="1000" r="565" fill="orange" />
				<path id="Terreno"
					d="M818.9,678.6c-14.3-18.6-14.8-49.5-31.4-66.1s-47.4-17.1-66.1-31.4c-18.6-14.3-27-43.9-47.4-55.7 c-20.2-11.7-50.1-4.2-71.9-13.3c-21.5-8.9-37.4-35.4-60.2-41.5c-22.5-6-49.4,9-72.9,5.9c-23-3-45.1-24.5-68.9-24.5 c-23.8,0-45.9,21.5-68.9,24.5c-23.5,3.1-50.4-11.9-72.9-5.9c-22.8,6.1-38.7,32.6-60.2,41.5c-21.8,9-51.7,1.6-71.9,13.3 c-20.4,11.8-28.8,41.5-47.4,55.7C60,595.5,29.2,596,12.6,612.6l862,113.4C862.8,705.6,833.1,697.2,818.9,678.6z"
					fill="#FC0" />
				<g class="PrimerPlano">
					<use xlink:href="#RuedaDelantera" class="Rodando Delantera" />
					<g class="Pedaleo">
						<line class="Pedal PedalI" x1="344" y1="309" x2="364" y2="309" />
						<line class="PalaPedal" x1="354" y1="309" x2="354" y2="359" />
					</g>
					<use xlink:href="#gAnterior" />
					<use xlink:href="#RuedaTrasera" class="Rodando Trasera" />
					<use xlink:href="#Cuadro" class="CuadroI" />
					<use xlink:href="#EstrellaCompleta" class="Pedaleo" />
					<circle class="Estrellita Dientes" cx="198" cy="401" r="6" stroke="#999" fill="#999" />
					<use xlink:href="#Cadena" class="CadenaA" />
					<use xlink:href="#Cadena" class="CadenaB" />
					<use xlink:href="#Cadena" class="CadenaC" />
					<use xlink:href="#Pinion" class="Rodando Trasera" />
					<polyline class="CuadroI" points="323.2,241.7 217.3,354.2 289.7,354.2 " stroke-width="11"
						stroke-linejoin="round" />
					<polyline class="Componentes" points="198,401 223,387 201,367 217,354 " stroke-width="6"
						stroke-linecap="round" />
					<g class="Pedaleo">
						<line class="PalaPedal" x1="354" y1="359" x2="354" y2="409" />
						<line class="Pedal PedalD" x1="344" y1="409" x2="364" y2="409" />
					</g>
				</g>
			</svg>
		</div>