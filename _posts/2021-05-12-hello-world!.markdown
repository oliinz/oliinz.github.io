---
layout: post
title:  "Hello World!"
date:   2021-08-01 20:13:52 +0800
categories: random
---

**CB Notes **

Hi, gumawa ako ng basic simulator chrome extension for Cryptoblades combat (Linked below). List ng mga na-discover ko & other things: 

1️⃣ Pag 100% chance of winning ka na ayon sa simulator, wala ka nang chance matalo kahit may randomness yung combat. Sa computation kasi ng roll ng enemy at hero, ang random lang is yung + or - 10%. So minsan makaka roll yung character mo ng -10%, or +8%. Same with the enemy. Sure win pag 100% na ang probability kase may times na kahit ang roll mo is -10%  tapos ang na roll ng enemy is +10%, mas mataas pa rin ang total roll mo. 

Example: 
```
Hero worst roll (-10%) = 4800 - 10% = 4320
Enemy best roll (+10%) = 3600 + 10% = 3960

100% chance of winning. Enemy will never roll a value greater than yours.
```
Dito, kahit ang naka kuha ka ng -10% , mas mataas pa rin nakuha mo kesa sa enemy na may +10% dahil sobrang baba ng stats niya or countered mo ang element niya.

2️⃣ Fire > Earth > Lightining > Water > Fire. A question I had as a newb:  pano kapag EARTH ang element ng hero ko tapos ang enemy ay Water, may effect ba ito sa random roll? Kasi base sa diagram *parang* mas malakas ang earth sa water since lightning is stronger than water tapos earth is stronger than lightning :thinking:

**answer:** Walang effect. Ang kinoconsider lang ng formula is yung weakness and strength ng isang element. Kung yung element ng hero mo ay strong against sa enemy, you get a bonus(+0.075), pero kung yung enemy element is stronger than your hero's element,  deduction (-0.075). 

You also get bonus if your hero's element is the same as your weapons **main** element (+0.0075).  

(Emoji-filled) Example: 
```
🔥 > 🌳 > ⚡ > 💦 > 🔥

HERO  +  WEAPON vs ENEMY = GOOD or BAD?

💦   +  💦  vs  🔥  =  GOOD 

🌳  +  💦  vs  🔥  = BAD 

⚡  +  🌳  vs  ⚡ = Not great, not terrible
```:sweat_drops::sweat_drops::sweat_drops::sweat_drops:

**Hindi guarantee yung good combination ng elements.** Kahit good combination yan, depende pa rin sa power ng enemy vs hero. See point #3️⃣.

Also, parang maliit lang yung 0.0075 pero **significant** siya. Kase yung roll mo is multiplied by 1 pero kung may + 0.0075 ka, multiplied by 1.0075 na ang roll mo. Even better kung 1.015 (hero element is directly stronger than enemy + weapon element is the same as hero element)

3️⃣ Kahit same element ang hero and weapon tapos countered ang enemy element, hindi pa rin sure na mataas ang probability of winning. Minsan kase masyadong mataas ang power ng enemy na kahit countered mo sya, malaki pa rin ang chance of losing. Kaya without the simulator, pwede ka ma-trap kung sa elements ka lang titingin.

4️⃣ "100% percent chance of winning daw, should I use 200 stamina?". 
Pag ni-run ko ang simulation ng ilang beses tapos 100% talaga, full 200 stamina na ginagamit ko.  Kahit mas mababa ang skill na makukuha (to compensate for the gas saved). This is just my personal opinion pero I'd rather lose some SKILL than spend BNB kase in my opinion, mas okay gastusin yung pera na nakuha ko sa game (SKILL) kesa maglabas pa ng pera pang gas (BNB). 

Pag meron nang opportunity para sa 100% win, grab ko na. 

**Reason:** Kase pano kung ang next set of enemies na ibigay sayo ay nasa 35-50% chance of winning lang (lahat sila counter sa element mo)? May risk na mawala ang profit mo para sa turn na 'yun. FEELING ko mas malaki ang reward ng one *talpak*200 stamina all win, vs 5 ~~talpak, rounds nalang ~~ rounds 40 stam na may 1 loss. 

Wala akong data to back this up and if anyone can prove me wrong, edit ko nalang. Help: Need real data. 

5️⃣ "98% chance daw, should I use 200 stamina?". 
I wouldn't risk it. Sayang. Don't underestimate the 2% or kahit 1% or whatever. If you lose, isipin mo nalang it's worth almost **A WHOLE DAY** of potential earnings. You can try it with 40 stamina, then hope na yung next batch na itho-throw sayo ni *KROGE*:kroge:  ay may 100%. 

You can also try to set to 80 or 120 stamina to save gas then hope you win. You save gas + you get to feel great for beating the 98% chance. I don't recommend doing this. Is it worth the risk of losing 2 rounds to save gas? No, unless masyadong mahal ang BNB for gas, I guess?  

6️⃣ I appreciate the oracle system. 
I don't know why others hate it, I may be missing something pero I think it's a great selling point for those looking to earn a little ~~hehe little lang daw~~. If I understand correctly, the oracle is there to keep the rewards, and in-game expenses consistent (in usd) no matter the price of SKILL. This is great since walang uncertainty sa spending and earning. You spend and earn the same amount in USD. I might be wrong though and you might not agree with me which is fine. I'm willing to accept corrections. Bummer they *overrode* it. I hope they fix it.

----------

📌 Link to the extension Github page: https://github.com/oliinz/cb-assistant 

About the extension: 
One-click tool that runs 1000 battle simulations against each enemy and returns the percentage of wins out of 1000 battles. 100% = 1000 out of 1000 battles won. Click the extension multiple times para sigurado sa percentage. More info on the github page linked above including installation, usage, and information on computation. For me, mas convenient ito kasi no need na to input things, or switch tab. Ping me or message me if you're having trouble with the installation.

*The extension is free and open source meaning anyone can see and audit the code to make sure that no malicious activities happen whether intended or not. It will never send **any data** to anyone or anything.*

*The information provided here are of my own. And though I aim for, I cannot guarantee factuality as these were derived from my own experiences and discoveries. The game updates frequently and some of the things I said here could be outdated in a day. DYOR.*

Thanks for reading 💙  ping me for any suggestions/clarifications/corrections
