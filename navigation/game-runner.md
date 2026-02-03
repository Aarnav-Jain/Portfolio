---
layout: post
codemirror: true
title: Game Runner Examples
description: Learn game development using the GameEngine framework in a contained educational environment. Build game levels, add characters, and create interactive experiences with live code editing and debugging controls.
permalink: /rpg/game

---

## Basic Game: Desert Adventure

{% capture challenge1 %}
Run the basic desert adventure game. Use WASD or arrow keys to move Chill Guy around the desert. Walk up to R2D2 to trigger a mini-game!
{% endcapture %}

{% capture code1 %}
import GameEnvBackground from '/assets/js/BetterGameEngine/essentials/GameEnvBackground.js';
import Player from '/assets/js/BetterGameEngine/gameObjects/Player.js';
import Npc from '/assets/js/BetterGameEngine/gameObjects/Npc.js';
import Barrier from '/assets/js/adventureGame/Barrier.js';

class CustomLevel {
        constructor(gameEnv) {
            const path = gameEnv.path;
            const width = gameEnv.innerWidth;
            const height = gameEnv.innerHeight;

            // Definitions will be added here per step

            // Define objects for this level progressively via Confirm Step
            this.classes = [
                // Step 1: add GameEnvBackground
                // Step 2: add Player
                // Step 3: add Npc
            ];
        }
    }

    export const gameLevelClasses = [CustomLevel];
export { GameControl };
export const gameLevelClasses = [CustomLevel];
{% endcapture %}

{% include game-runner.html
   runner_id="game1"
   challenge=challenge1
   code=code1
   height="150px"
%}
