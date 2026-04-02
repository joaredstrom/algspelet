# Algspelet

---

## :sweden: Svenska

Ett spel for tva spelare dar alger vaxer upp fran havsbotten och man ska trycka pa dem innan de forsvinner!

Byggt med HTML, CSS och JavaScript. Ingen framework behovs.

### Funktioner

- Alger som vaxer upp som sjogras fran havsbotten pa slumpmassiga stallen
- Tva spelare pa delad skarm med en rod linje i mitten
- Explosion med ljud nar man triffar en alg
- "Eeeoo"-ljud nar alger vaxer upp och ner
- Forsta spelaren till 30 poang vinner
- Det blir svarare - fler och fler alger dyker upp
- Havsbotten-bakgrund med bubblor

### Barnets instruktioner

#### Grundidén

> Forst ska det vaxa upp snabbt lite alger och sen ska de aka ner igen, och man ska forsoka trycka pa dem och sa forsvinner dem.

#### Mina foljdfragor och svar

- **Var ska algerna vaxa ifran?** - Pa alla mojliga olika stallen
- **Hur ska algerna se ut?** - Som vanliga alger, som sjogras
- **Hur snabbt aker de ner igen?** - Man ska hinna se dem ett tag
- **Vad hander nar man trycker pa en alg?** - Det ska vara en explosion som man ser och sa hor man det. Det ska ocksa lata nar de aker upp och ner, eeeoo upp och ner
- **Ska man fa poang?** - Ja
- **Kommer det fler och fler alger?** - Ja det ska komma fler och fler
- **Ska spelet ha en bakgrund?** - Havsbotten

Barnet la ocksa till:

> Det ska ocksa vara tva spelare

- **Tva spelare pa samma skarm?** - Halva skarmen var, en rod linje i mitten
- **Hur vet man vem som tryckte?** - Olika farger och olika sidor
- **Hur lange pagar spelet?** - Den som forst far 30
- **Vem vinner?** - Den som forst far 30
- **Ska det finnas en startskarm?** - Borja direkt

### Hur instruktionerna blev till kod

Har ar vad Claude gjorde for att instruktionerna skulle bli verklighet:

#### 1. Skapa havsbotten

Bakgrunden ar en gradient som gar fran morkt bla hogst upp (vattnet) ner till brunt langst ner (havsbotten). Det finns ocksa sma bubblor som stiger uppat for att det ska kanna mer som under vattnet.

#### 2. Fa alger att vaxa

Varje alg ar en gron stam som vaxer uppat med sma blad pa sidan - precis som sjogras. De dyker upp pa slumpmassiga stallen, vaxer upp, stannar kvar ett tag, och krymper sedan tillbaka ner. De vajar lite fram och tillbaka for att kanna mer levande.

#### 3. Ljuden - eeeoo

Barnet ville att det skulle lata "eeeoo" nar algerna aker upp och ner. Claude anvande Web Audio API for att skapa en ton som glider uppat (eee) nar algen vaxer och nedat (ooo) nar den krymper. Nar man traffar en alg hors ett explosionsljud (vitt brus som tynar bort snabbt).

#### 4. Tva spelare

Skarmen ar delad pa mitten med en rod linje. Spelare 1 (bla) spelar pa vanster sida och spelare 2 (orange) spelar pa hoger sida. Alger dyker upp pa bada sidor och varje spelare kan bara trycka pa alger pa sin egen sida.

#### 5. Poang och vinst

Varje gang man trycker pa en alg far man ett poang och poangen studsar till lite for att det ska kannas bra. Den som forst nar 30 poang vinner och da visas en vinnarskarm med en "Spela igen"-knapp.

#### 6. Svårare och svarare

I borjan dyker det upp en ny alg ungefar varannan sekund. Var femte sekund okar takten sa att alger dyker upp oftare och oftare. Tillslut kommer de sa snabbt att det ar riktigt svart att hinna med!

---

## :gb: English

A two-player game where seaweed grows up from the ocean floor and you have to tap it before it disappears!

Built with HTML, CSS and JavaScript. No framework needed.

### Features

- Seaweed that grows up from the ocean floor in random places
- Two players on a split screen with a red line in the middle
- Explosion with sound when you hit a seaweed
- "Eeeoo" sound when seaweed grows up and down
- First player to 30 points wins
- It gets harder - more and more seaweed appears
- Ocean floor background with bubbles

### The child's instructions

#### The basic idea

> First some seaweed should grow up quickly and then go back down again, and you should try to tap them and then they disappear.

#### My follow-up questions and answers

- **Where should the seaweed grow from?** - In all sorts of different places
- **What should the seaweed look like?** - Like regular seaweed, like sea grass
- **How fast do they go back down?** - You should have time to see them for a while
- **What happens when you tap a seaweed?** - There should be an explosion that you see and you hear it. It should also make a sound when they go up and down, eeeoo up and down
- **Should you get points?** - Yes
- **Do more and more seaweed appear?** - Yes, more and more should come
- **Should the game have a background?** - Ocean floor

The child also added:

> There should also be two players

- **Two players on the same screen?** - Half the screen each, a red line in the middle
- **How do you know who tapped?** - Different colors and different sides
- **How long does the game last?** - The one who first gets 30
- **Who wins?** - The one who first gets 30
- **Should there be a start screen?** - Start immediately

### How the instructions became code

Here is what Claude did to make the instructions become reality:

#### 1. Create the ocean floor

The background is a gradient that goes from dark blue at the top (the water) down to brown at the bottom (the ocean floor). There are also small bubbles rising upwards to make it feel more like being underwater.

#### 2. Make seaweed grow

Each seaweed is a green stem that grows upward with small leaves on the side - just like sea grass. They appear in random places, grow up, stay for a while, and then shrink back down. They sway slightly back and forth to feel more alive.

#### 3. The sounds - eeeoo

The child wanted it to sound "eeeoo" when the seaweed goes up and down. Claude used the Web Audio API to create a tone that slides upward (eee) when the seaweed grows and downward (ooo) when it shrinks. When you hit a seaweed, an explosion sound plays (white noise that fades quickly).

#### 4. Two players

The screen is split in the middle with a red line. Player 1 (blue) plays on the left side and Player 2 (orange) plays on the right side. Seaweed appears on both sides and each player can only tap seaweed on their own side.

#### 5. Points and winning

Every time you tap a seaweed you get a point and the score bounces a little to make it feel good. The first player to reach 30 points wins and a winner screen is shown with a "Play again" button.

#### 6. Harder and harder

In the beginning, a new seaweed appears roughly every two seconds. Every five seconds the pace increases so that seaweed appears more and more frequently. Eventually they come so fast that it's really hard to keep up!
