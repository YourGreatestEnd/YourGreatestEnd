/* ----------------------------------------------------------------- HUD -- */

#best_streak_container {
    position: absolute;
	top: var(--ss-space-sm); left: 50%;
	padding: 0; margin: 0;
    transform: translateX(-50%);
	text-align: center;
	z-index: 6;
}

#best_streak_container h1 {
	margin: 0; padding: 0;
	display: inline;

	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);

	font-family: 'Nunito', sans-serif !important;
	font-size: 2.5em !important;
	color: var(--ss-white) !important;
	font-weight: bold !important;
	text-transform: lowercase;

	padding-left: 1.25em;
	padding-top: 0em;

	background-image: url('https://cdn.discordapp.com/attachments/965451008736104498/965543282883051570/7b4f5fb2785f755a831f3697517abe41--enderman-minecraft-minecraft-room.jpg');
    background-position: left;
	background-size: 50%;
    background-repeat: no-repeat;
}

#teamScores {
	transform: translateX(-50%);
	top: 0;
	left: 50%;
	display: none;
	position: absolute;
	z-index: 6;
}

#weaponBox {
	display: none; 
	position: absolute; 
	right: 0.75em; 
	bottom: 0.5em; 
	text-align: right;
}

#grenades {
	padding-bottom: 0; 
	margin-bottom: 0;
}

#grenades img {
	width: 3.25em;
	height: auto;
}

#weaponName {
	text-align: right;
	font-family: 'Nunito', sans-serif;
	font-weight: bold;
	line-height: 0;
	display: none;
}

#ammo {
	text-align: right;
	font-size: 3.25em;
	font-family: 'Nunito', sans-serif;
	font-weight: bold;
	line-height: 1em;
	margin: 0;
	
	padding-right: 1.2em;
	padding-top: 0em;
	margin-bottom: 0.1em;

	background-image: url(../img/ico_ammo.png);
    background-position: right center;
	background-size: contain;
    background-repeat: no-repeat;
}

#healthContainer {
	position: absolute;
	left: 50%; bottom: 1em;
	transform: translateX(-50%);
	display: inline-block;
	width: 6em; height: 6em;
	background: var(--ss-blueshadow);
	border-radius: 50%;
	text-align: center;
}

#health {
}

#healthHp {
	font-family: 'Nunito', sans-serif;
    font-weight: bold;
    color: var(--ss-white);/*#2390c9;*/
    font-size: 1.2em;
    transform: translateY(-3.45em);
}

.healthBar {
	transform-origin: center;
	transform: rotate(90deg);
	fill: transparent;
	stroke: #2390c9;
	stroke-width: 1em;
	stroke-dasharray: 14.4513em;
	transition: all 0.3s ease-in-out;
}

.healthYolk {
	fill: #096a95;/*#0886bf;*/
}

.healthSvg {
	width: 100%; height: 100%;
}

#hardBoiledContainer {
	position: absolute;
	left: 50%; bottom: 1em;
	transform: translateX(-50%);
	display: inline-block;
	width: 6em; height: 6em;
	text-align: center;
}

#hardBoiledValue {
	font-family: 'Nunito', sans-serif;
    font-weight: bold;
    color: var(--ss-white);
    font-size: 1.6em;
    transform: translateY(-2.6em);
}

#hardBoiledShieldContainer {
	width: 100%;
	height: 100%;
}

.hardBoiledShield {
	position: absolute;
	transform: translateX(-50%);
	height: 100%;
}

#eggBreakerContainer {
	position: absolute;
	left: calc(50% + 9em); bottom: 1em;
	transform: scale(4) translateY(-3em);
	transform-origin: 50% 100%;
	width: 6em; height: 6em;
}

#eggBreakerContainer.on {
	visibility: visible;
	transform: scale(1) translateY(0);
	transition: 1s;
}

#eggBreakerContainer.off {
	visibility: hidden;
}

#eggBreakerIcon {
	position: absolute;
	height: 100%;
}

#eggBreakerTimer {
	position: absolute;
	color: white;
	text-shadow: var(--ss-yolk) 0 0 0.1em, black 0 0.1em 0.2em;
	font-size: 2.5em;
	font-family: 'Nunito', sans-serif;
	font-weight: 900;
	text-align: center;
	width: 100%;
	top: 24%;
}

#shellStreakContainer {
    position: absolute;
    top: 18%;
    left: 50%;
	transform: translateX(-50%);
	text-align: center;
	z-index: 6;
}

#shellStreakCaption {
	color: var(--ss-white);
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
	margin: 0;
}

#shellStreakMessage {
	color: var(--ss-white);
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
	font-size: 2.5em;
	margin: 0;
}

#shellStreakMessage.appear {
    visibility: visible;
    transform: scale(1);
    transition: 0.5s;
}

#shellStreakMessage.disappear {
    visibility: hidden;
    transform: scale(2);
}

@keyframes shellStreakMessage {
    from {
        transform: scale(0) rotate(0deg);
        opaity: 1;
    }

    10% {
        transform: scale(2) rotate(360deg);
        opacity: 1;

    }

    15% {
        transform: scale(1) rotate(360deg);
    }

    85% {
        opacity: 1;
        transform: scale(1) translateY(0) rotate(360deg);
    }

    to {
        opacity: 0;
        transform: scale(1) translateY(10em) rotate(360deg);
    }
}

#grenadeThrowContainer {
	position: absolute;
	display: flex;
	visibility: hidden;
	align-items: flex-end;
	top: 50%;
	left: 50%;
	transform: translate(-6em, -3em);
	width: 1em;
	height: 6em;
	background: rgba(0, 0, 0, 0.25);
	border-radius: 0.3em;
	padding: 0.25em;
}

#grenadeThrow {
	width: 100%;
	height: 50%;
	border-radius: 0.05em;
	background: white;
}

#killBox {
	position: absolute;
	display: none;
	width: 100%;
	transform-origin: center bottom;
	bottom: 20%;
	color: var(--ss-white);
	text-align: center;
}

#KILL_STREAK {
	font-style: italic;
}


#KILL_STREAK,
.game-start-loading-message,
.game-start-loading-message h3 {
	text-align: center;
}

.game-start-loading-message,
.game-start-loading-message h3 {
	width: 100%;
	display: block;
}

.game-start-loading-message,
.btn__respawning {
	min-height: 7em;
}

#killBox h3, #deathBox h3 {
	font-weight: 900;
	margin: 0;
	color: var(--ss-white);
	font-family: 'Nunito', sans-serif;
}

#killBox h2, #deathBox h2 {
	font-size: 2em; 
	line-height: 1em;
	margin: 0;
	font-weight: 900;
	color: var(--ss-white);
	font-family: 'Nunito', sans-serif;
	text-transform: none !important;
}

#deathBox {
	position: absolute;
	display: none;
	width: 100%;
	transform-origin: center top;
	top: 20%;
	color: #fff;
	text-align: center;
}

#gameMessage {
	position: absolute;
	visibility: hidden;
	top: 60%; left: 50%;
	transform: translateX(-50%);
	color: #fff;
	font-weight: bold;
	font-size: 1.5em;
	text-align: center;
	z-index: 6;
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
}

#gameMessage.show {
	visibility: visible;
	animation: 2.5s gameMessage forwards;
}

#gameMessage.hide {
	visibility: hidden;
}

@keyframes gameMessage {
	0% { transform: translateX(-50%) scale(0); }
	10% { transform: translateX(-50%) scale(1.4); }
	15% { transform: translateX(-50%) scale(1); }
	20% { transform: translateX(-50%) scale(1.2); }
	25% { transform: translateX(-50%) scale(1); }
	30% { transform: translateX(-50%) scale(1.1); }
	35% { transform: translateX(-50%) scale(1); }
	90% { transform: translateX(-50%) scale(1); }
	100% { transform: translateX(-50%) scale(0); visibility: hidden }
}

.chat {
	position: absolute;
	font-weight: bold;
	color: var(--ss-white);
	z-index: 6;
}

#chatOut {
	display: none;
	bottom: 2.5em;
	left: 1em;

}

#chatIn {
	display: none;
	color: #ff0;
	bottom: 1em;
	left: 1em;
	width: 30%;
	border: none;
	background: none;
}

#killTicker {
	position: absolute;
	text-align: right;
	right: 1em;
	top: 10em;
	height: 7em;
	transform-origin: top right;
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
}

#playerList {
	display: table;
	border-collapse: separate;
	border-spacing: 0.2em;
	position: absolute;
	left: 1em; top: 1em;
	z-index: 6;
	width: 12em;
}

#spectate {
	display: none;
	position: absolute;
	right: 1em;
	bottom: 1em;
	text-align: center;
	padding: 0.5em 1em 0.5em 1em;
	border-radius: 0.3em;
	font-weight: bold;
	color: var(--ss-white);
	background: rgba(0, 0, 0, 0.3);
}

#serverAndMapInfo {
	position: absolute;
	right: var(--ss-space-sm);
	bottom: var(--ss-space-sm);
	text-align: right;
	color: var(--ss-white);
	font-weight: bold;
	font-size: 1.4em;
	line-height: 1em;
	z-index: 6;
}

#inGameUI {
	position: absolute; right: 0.3em; top: 0em;
}

#readouts {
	position: absolute;
	top: 2.2em;
	right: 0em;
	display: block; 
	text-align: right; 
	color: var(--ss-white);
	font-weight: bold;
	clear: both;
	font-size: 1.3em !important;
	text-transform: uppercase;
	line-height: 1em;
	white-space: nowrap;
	z-index: 6;
}

#readouts div {
	display: inline;
	font-size: 1em !important;
	margin-left: 0.1em;
}

#game_account_panel {
	z-index: 6;
	width: auto;
	position: absolute;
	top: var(--ss-space-sm);
	right: var(--ss-space-sm);
}

#chickenBadge {
	position: absolute;
	top: 5.25em;
	width: 5em;
	height: 5em;
	right: var(--ss-space-sm);
	z-index: 6;
}

#chickenBadge img {
	width: 100%;
	height: 100%;
}

#scopeBorder {
	box-sizing: initial;
	display: flex;
	flex-direction: row;
	justify-content: center;
	width: 100vw; height: 100vh;
	position: absolute;
	top: 0px; left: 0px;
	pointer-events: none;
	overflow-x: hidden;
}

#maskleft, #maskright {
	background: var(--ss-black);
	flex: 1;
}

#maskmiddle {
	background: url('https://cdn.discordapp.com/attachments/743631842527150122/954343221088092220/scope.png') center center no-repeat;
	background-size: contain;
	width: 100vh;
	height: 100vh;
}

.crosshair {
	position: absolute;
	transform-origin: 50% top;
	top: 50%;
	border: solid 0.05em black;
	height: 0.8em;
	margin-bottom: 0.12em;
	opacity: 0.7;
}

.crosshair.normal {
	left: calc(50% - 0.15em);
	background: white;
	width: 0.3em;
}

.crosshair.powerful {
	left: calc(50% - 0.25em);
	background: red;
	width: 0.5em;
}

#dotReticle {
	position: absolute;
	left: 50%; top: 50%;
	transform: translate(-50%, -50%);
	background: var(--ss-yolk);
	width: 0.7em; height: 0.7em;
	border-radius: 100%;
}

#shotReticleContainer {
	position: absolute;
	text-align: center;
	left: 50%; top: 50%;
	transform: translate(-50%, -50%);
	opacity: 0.7;
	overflow-x: hidden;
}

#reticleContainer {
	position: fixed;
	top: 0; left: 0;
	width: 100%; height: 100%;
}

#crosshairContainer {
	position: absolute;
	left: 50%; top: 50%;
	transform: perspective(0px);
}

.shotReticle {
	box-sizing: border-box;
	position: absolute;
	left: 50%;
	width: 2.5em;
	height: 100%;
	transform-origin: center;
	background: transparent;
	border: solid;
	border-left: solid transparent;
	border-right: solid transparent;
	border-radius: 1.25em 1.25em 1.25em 1.25em;
}

.shotReticle:nth-child(1n) {
	transform: translateX(-50%) rotate(0deg);
}

.shotReticle:nth-child(2n) {
	transform: translateX(-50%) rotate(90deg);
}

.shotReticle.fill {
}

.shotReticle.border {
}

.shotReticle.fill.normal {
	border-color: white;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.1em;
	padding: 0.1em;
}

.shotReticle.fill.powerful {
	border-color: red;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.3em;
	padding: 0.1em;
}

.shotReticle.border.normal {
	border-color: black;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.2em;
}

.shotReticle.border.powerful {
	border-color: black;
	border-left: solid transparent;
	border-right: solid transparent;
	border-width: 0.4em;
}


@keyframes armed {
    0% { transform: translate(-50%, -50%) scale(1.25); }
    100% { transform: translate(-50%, -50%) scale(1); }
}

@keyframes unarmed {
    0% { transform: translate(-50%, -50%) scale(0.8); }
    100% { transform: translate(-50%, -50%) scale(1); }
}

#readyBrackets {
	position: absolute;
	left: 50%; top: 50%;
	transform: translate(-50%, -50%);
	opacity: 0.5;
}

#readyBrackets.ready {
	animation: armed 0.2s linear;
	width: 4em; height: 4em;
	border-color: rgb(0, 255, 0);
}

#readyBrackets.notReady {
	animation: unarmed 0.2s linear;
	width: 8em; height: 8em;
	border-color: rgb(255, 0, 0);
}

.readyBracket {
	position: absolute;
	width: 0.8em; height: 0.8em;
	border: solid;
	border-color: inherit;
	border-width: 0.3em 0 0 0.3em;
	transform-origin: top left;
}

.readyBracket:nth-child(1) {
	left: 100%;
	transform: rotate(90deg);
}

.readyBracket:nth-child(2) {
	left: 100%; top: 100%;
	transform: rotate(180deg);
}

.readyBracket:nth-child(3) {
	top: 100%;
	transform: rotate(270deg);
}

#spatulaPlayer {
	display: none;
    position: absolute;
    width: 2.8em;
    left: 50%;
    bottom: 1.4em;
    transform: translateX(4.5em);
    transform-origin: center bottom;
}

#spatulaPlayer.capture {
	display: block;
	animation: spatulaPlayerCapture 0.5s ease-in-out;
}

#spatulaPlayer.drop {
	display: none;
}

@keyframes spatulaPlayerCapture {
	from {
		opacity: 0;
		transform: translate(0, 0) scale(6);
	}

	to {
		opacity: 1;
		transform: translate(4.5em, 0) scale(1) ;
	}
}

#captureContainer {
	white-space: nowrap;
	position: absolute;
	left: 50%;
	top: 3.5em;
	transform: translateX(-50%);
	padding: 0;
	font-family: 'Nunito', sans-serif;
	font-weight: 900;
}
 
#captureCenter {
	display: inline-block;
	text-align: center;
}

#captureBarContainer {
	width: 20em;
	height: 3em;
	background: rgba(0, 0, 0, 0.7);
	border-radius: 2em 2em 2em 2em;
	border: solid 0.5em rgba(255, 255, 255, 0.3);
	overflow: hidden;
}

#captureBar {
	width: 19em;
	height: 3em;
	transform-origin: left;
	transform: scaleX(100%);
}
  
#captureBarText {
	color: white;
	font-size: 1.25em;
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
}

.captureCrown {
	height: 3em;
}

.captureScoreContainer {
	display: inline-block;
	text-align: center;
}
  
.captureScore {
	color: white;
	font-size: 1.5em;
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
}

#captureBar.empty {
	visibility: hidden;
}

#captureBar.contested {
	animation: contestedBar 300ms infinite alternate;
}

@keyframes contestedBar {
	0% { background: var(--ss-team-blue-light) }
	100% { background: var(--ss-team-red-light) }
}

#captureBar.takeover {
	background: white;
}

#captureBar.blue {
	background: var(--ss-team-blue-light);
}

#captureBar.red {
	background: var(--ss-team-red-light);
}

#captureBar.blueAbandoned {
	background: var(--ss-team-blue-dark);
}

#captureBar.redAbandoned {
	background: var(--ss-team-red-dark);
}

#captureIconContainer {
	position: fixed;
	transform: translate(-50%, -50%);
	visibility: hidden;
}

#captureIconContainer.on {
	visibility: visible;
}

#captureInsideContainer {
	transform: translate(-50%, -50%);
	text-align: center;
}

#captureIconCaption {
	color: white;
	font-size: 1.5em;
	font-weight: 900;
	transform: translateY(-0.2em);
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
}

#captureIcon.empty {
	fill: black;
}

#captureIcon.contested {
	animation: contestedIcon 300ms infinite alternate;
}

@keyframes contestedIcon {
	0% { fill: var(--ss-team-blue-light) }
	100% { fill: var(--ss-team-red-light) }
}

#captureIcon.takeover {
	fill: rgb(225, 225, 225);
}

#captureIcon.blue {
	fill: var(--ss-team-blue-light);
}

#captureIcon.red {
	fill: var(--ss-team-red-light);
}

#captureIcon.blueAbandoned {
	fill: var(--ss-team-blue-dark);
}

#captureIcon.redAbandoned {
	fill: var(--ss-team-red-dark);
}

#captureIcon {
	position: absolute;
	height: 3em;
	top: 3.8em;
	left: 1.1em;
}

#captureRingBackground {
	position: absolute;
	width: 6.5em;
	height: 6.5em;
	border: solid .5em black;
	box-shadow: 0 0 0 0.15em inset rgba(0, 0, 0, 0.5),  0 0 0 0.15em rgba(0, 0, 0, 0.5);
	border-radius: 7em;
}

#captureRingContainer {
	position: relative;
	width: 6.5em;
	height: 6.5em;
	overflow: hidden;
	transform: translateY(20%);
}

#captureRing {
	position: absolute;
	width: 6.5em;
	height: 6.5em;
	border: solid 0.5em red;
	border-radius: 7em;
	transform: translateY(-20%);
}

#captureRing.empty {
	visibility: hidden;
}

#captureRing.contested {
	animation: contestedRing 300ms infinite alternate;
}

@keyframes contestedRing {
	0% { border-color: var(--ss-team-blue-light) }
	100% { border-color: var(--ss-team-red-light) }
}

#captureRing.takeover {
	border-color: rgb(225, 225, 225);
}

#captureRing.blue {
	border-color: var(--ss-team-blue-light);
}

#captureRing.red {
	border-color: var(--ss-team-red-light);
}

#captureRing.blueAbandoned {
	border-color: var(--ss-team-blue-dark);
}

#captureRing.redAbandoned {
	border-color: var(--ss-team-red-dark);
}

#bigMessageContainer {
	position: absolute;
	top: 50%;
	width: 100%;
	transform: translateY(-50%);
	text-align: center;
	color: white;
}

#bigMessage {
	position: absolute;
	left: 50%;
	animation: bigMessage 4500ms linear 300ms forwards;
	visibility: hidden;
}

.bigMessageText {
	white-space: nowrap;
	font-family: 'Sigmar One', sans-serif;
	font-size: 6em;
	font-style: italic;
}

@keyframes bigMessage {
	0% {
		visibility: visible;
		transform: scaleX(0) translateX(50vw);
		transform-origin: center;
		opacity: 0;
	}

	7% {
		transform: scaleX(1) translateX(-47%);
		transform-origin: center;
		opacity: 1;
	}

	93% {
		transform: scaleX(1) translateX(-53%);
		opacity: 1;
	}

	100% {
		transform: translateX(-100vw);
		transform-origin: left;
		opacity: 0;
	}
}

#bigMessageCaption {
	margin-top: 5.5em;
	font-size: 1.5em;
	font-weight: bold;
	animation: bigMessageCaption 3400ms linear 1000ms forwards;
	visibility: hidden;
	color: rgb(255, 192, 50);
}

@keyframes bigMessageCaption {
	0% {
		visibility: visible;
		opacity: 0;
		transform: scale(0);
	}

	5% {
		opacity: 1;
		transform: scale(1);
	}

	95% {
		opacity: 1;
		transform: scale(1);
	}

	100% {
		opacity: 0;
		transform: scale(0);
	}
}

#bigMessageBar {
	position: absolute;
	width: 100%;
	height: 14em;
	background: white;
	border-top: solid white 1em;
	border-bottom: solid white 1em;
	animation: bigMessageBar 5000ms ease-out forwards;
	transform-origin: top;
	box-shadow: 0 0 1em rgb(255, 255, 255);
}

@keyframes bigMessageBar {
	0% {
		transform: scale(0, 0.1) translateY(-50%) perspective(1px) translateZ(0);
	}
	
	5% {
		transform: scale(1, 0.1) translateY(-50%) perspective(1px) translateZ(0);
		background: white;
		border-color: white;
	}

	10% {
		transform: scaleY(1) translateY(-50%) perspective(1px) translateZ(0);
		background: rgba(0, 0, 0, 0.75);
		border-color: var(--ss-big-message-border-color);
	}

	95% {
		transform: scaleY(1) translateY(-50%) perspective(1px) translateZ(0);
		background: rgba(0, 0, 0, 0.75);
		border-color: var(--ss-big-message-border-color);
	}

	100% {
		transform: scale(1, 0) translateY(-50%) perspective(1px) translateZ(0);
		background: white;
		border-color: white;
	}
}

.teamScore {
	position: absolute;
	width: 12vh;
	height: 8vh;
	top: 0.5em;
	padding: 2vh;
	box-sizing: border-box;
	border: solid rgba(0, 0, 0, 0.5);
	text-shadow: none;
	text-align: center;
	z-index: 6;
}

.teamScore.red {
	border-radius: 7vh 5vh 5vh 7vh / 4vh 4vh 4vh 4vh;
	border-right-width: 4vh;
	transform: translateX(-22vh);
}

.teamScore.blue {
	border-radius: 5vh 7vh 7vh 5vh / 4vh 4vh 4vh 4vh;
	border-left-width: 4vh;
	transform: translateX(10vh);
}

.teamScore.active {
	opacity: 1;
}

.teamScore.inactive {
	opacity: 0.5;
}

.teamScore.red.active {
	color: #fff;
	background: rgba(255, 0, 0, 0.7);
}

.teamScore.red.inactive {
	color: #f00;
	background: rgba(64, 0, 0, 0.7);
}

.teamScore.blue.active {
	color: #fff;
	background: rgba(0, 128, 255, 0.7);
}

.teamScore.blue.inactive {
	color: #0af;
	background: rgba(0, 32, 64, 0.7);
}

.teamScore .number {
	width: 100%;
	position: absolute;
	margin-left: -2vh;
	font-size: 3vh;
	font-weight: bold;
}

.teamLetter.red {
	position: absolute;
	font-size: 3vh;
	right: -0.9em;
	font-weight: bold;
}

.teamLetter.blue {
	position: absolute;
	font-size: 3vh;
	left: -0.9em;
	font-weight: bold;
}
#inGameScaler, #inGameScaler .pause-btn-group {
	margin-right: 1em;
}
#inGameScaler {
	display: flex;
	flex-wrap: nowrap;
	align-items: baseline;
    margin: auto;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
}
#pausePopup, .player__container {
	position: relative;
}
.player__container {
	margin: var(--ss-space-lg) var(--ss-space-lg) 0 var(--ss-space-lg);
	height: 50vh;
	flex: 0 0 200px;
	max-width: 200px;
	align-self: flex-start;
	position: absolute;
	top: 0;
	left: 0;
}
.pause-popup--container {
    display: grid;
    width: auto;
    grid-template-columns: 15.5em 43em 26em;
    margin-top: 8em;
    margin-right: auto;
	margin-left: auto;
    grid-gap: 2em;
}
.pause-popup--container .fullwidth {
	width: auto !important;
	max-width: none !important;
}
#pausePopup {
	top: auto;
	left: auto;
	transform: none;
	/* width: 970px; */
	/* width: 70em; */
	width: auto;
	padding: var(--ss-space-md);
	min-height: 17.7em;
	display: flex;
	justify-content: center;
    margin-right: auto;
	margin-left: auto;
	grid-column: 2 / span 1;
    align-self: center;
}

.pause-btn-group .ss_button {
	text-align: left;
	margin: 0 0 var(--ss-space-sm) 0;
	margin-bottom: .5em;
	height: 2.3em;	
}
.pause-bg #weapon_select {
	flex-wrap: nowrap;
	justify-content: center;
	margin-bottom: 0
}

#game-play-switch {
	margin-top: 0;
}

.weapon-select--title h1 {
    color: var(--ss-white);
    background: none;
	padding: 0;
	margin: 0;
}

/* @media screen and ( max-height: 690px ), screen and (max-width: 995px) {
	.playing-poki .pause-popup--container {
		margin-right: auto;
		margin-left: 36em;
	}
} */
@media only screen and (min-width: 1420px)  {
	#inGameScaler {
		margin: 0 auto;
		float: none;
	}
}

#pausePopupInnards {
	width: 100%;
}
#pauseAdPlacement,
.pauseFiller {
	position: relative;
	z-index: 10;
	margin-right: auto;
	margin-left: auto;
	/* min-width: 40em; */
    display: flex;
}
.pauseFiller.shellshockers-respawn-banner-2 {
	min-width: auto;
}
#pauseAdPlacement iframe,
.pauseFiller iframe{
	margin: 0 auto;
	display: block;
	/*position: absolute;
	transform-origin: left top;
	transform: translateX(-50%);*/
}

.display-ad-container > div,
.display-ad-container > img {
	margin: 0 auto;
}

.respawn-container {
	display: block;
	margin: 0 auto;
}

.respawn-one {
    grid-column: 1 / span 3;
    display: block;
	margin: 0 auto;
    z-index: 6;
	position: relative;
	min-height: 10em;
}

.respawn-two {
	margin: 0;
    grid-column: 3 / span 1;
}

@media only screen and (max-width: 1200px)  {
	.playing-poki #div-gpt-ad-ShellShock_Respawn_Banner {
		margin: 0;
	}
}
#playerList {
	display: table;
	border-collapse: separate;
	border-spacing: 0.2em;
	position: absolute;
	left: 0; top: 0;
	z-index: 6;
}

.playerSlot {
	position: relative;
	margin-bottom: .2em;
}

.playerSlot--icons {
	width: 2.7em;
    display: block;
    position: absolute;
	right: -3.1em;
	top: 0;
	color: var(--ss-white)
}

.playerSlot--icons .hidden {
	display: none;
}

.playerSlot--icons i {
	margin-right: .2em;
}

.playerSlot--icons .vip-egg {
	text-shadow: 1px 1px 2px rgb(0 0 0 / 50%);
}

.playerSlot--name-score {
	display: block;
	width: 12em;
	padding: 0.05em 0.5em 0.05em 0.5em;
	border-radius: 0.2em;
	overflow-y: hidden;
	font-weight: 600;
}
.playerSlot--score {
	font-weight: 900;
	padding-left: 1em;
}

.playerSlot--name-score,
.btn-container {
	display: flex !important;
	justify-content: space-between !important;
	white-space: nowrap;
}
.playerSlot-player-is-me {
	background: var(--ss-me-player-bg);
	color: var(--ss-white-90);
}
.playerSlot-player-is-me.playerSlot-me-red {
	background: var(--ss-team-red-light-trans);
}
.playerSlot-player-is-me.playerSlot-me-blue {
	background: var(--ss-team-blue-light-trans);
}
.playerSlot-player-is-them {
	color: var(--ss-white-60);
}
.playerSlot-them {
	background: var(--ss-shadow);
}
.playerSlot-them-blue {
	background: var(--ss-team-blue-dark-trans);
	color: var(--ss-team-blue-light);
}
.playerSlot-them-red {
	background: var(--ss-team-red-dark-trans);
	color: var(--ss-team-red-light);
}

.player-action-vip-img img {
	width: 5em;
}

.vip-member-wrapper {
    margin: 1em auto;
}

#btn_horizontal.pause-popup--btn-group {
	flex-direction: column;
	/* max-width: 17.5em; */
	min-height: 6em;
	margin-top: 0;
}
.pause-popup--btn-group .ss_button.btn__respawning,
#btn_horizontal.pause-popup--btn-group {
	margin-right: auto;
	margin-left: auto;
}

.btn__respawning {
	border-radius: var(--ss-space-sm);
	border: none;
	background: var(--ss-yolk);
	color: var(--ss-white);
	text-align: center;
	font-weight: bold;
	line-height: 1em;
	padding: var(--ss-space-sm) var(--ss-space-lg);
	margin: 0 auto var(--ss-space-md) auto;
	white-space: nowrap;
}
.pause-popup--btn-group .ss_button:first-child {
	margin-left: 0 !important;
}
.pause-popup--btn-group .ss_button {
    margin: 0 0 0 0 !important;
}
.btn__team_switch {
	line-height: 3.9;
	font-size: .8em;
	margin-right: 1em;
}
.btn__team_switch i {
	font-style: italic;
}

/* ----------------------------------------------------------------- poki stuff -- */
.poki-reward-container {
    display: flex;
    justify-content: center;
}

.btn_reward {
	background-color: var(--ss-blue2);
	display: flex;
	align-items: center;
	text-shadow: var(--ss-space-micro) var(--ss-space-micro) var(--ss-shadow);
}

.playing-poki #inGameScaler {
	width: auto;
	float: none;
	margin: 0 auto;
}

.playing-poki .respawn-container {
    flex: 0 0 100%;
    display: flex;
    justify-content: center;
}
/**** Display ad *****/

#game_screen #event-notifications {
    margin: 0;
    position: absolute;
    z-index: 5;
	top: .8em;
	left: 50%;
	-webkit-transform: translateX(-50%);
	transform: translateX(-50%)
}
#game_screen #event-notifications img {
	height: 3em;
	width: auto;
}

/** start refactoring css */

.w-shrinkauto {
	flex: 1 0 auto;
}

@media only screen and (max-width: 1330px)  {
	.pause-popup--container {
		margin-top: 5em
	}
	.respawn-one {
		grid-column: 1 / span 3;
		margin: 0;
	}
}

@media only screen and (max-width: 922px)  {
	.pause-popup--container {
		/* This will correct the some impression issues but it also covers the player list */
		/* grid-template-columns: 11.5em 43em 35em;
		grid-gap: 1em; */
		grid-template-columns: 9.5em 43em 35em;
	}
}
