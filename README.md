# Algspelet

---

## :sweden: Svenska

Ett spel för två spelare där alger växer upp från havsbotten och man ska trycka på dem innan de försvinner!

Byggt med HTML, CSS och JavaScript med hjälp av Claude Opus 4.6 (claude-opus-4-6) via Claude Code. Ingen framework behövs.

### Funktioner

- Alger som växer upp som sjögräs från havsbotten på slumpmässiga ställen
- Två spelare på delad skärm med en röd linje i mitten
- Explosion med ljud när man träffar en alg
- "Eeeoo"-ljud när alger växer upp och ner
- Första spelaren till 30 poäng vinner
- Det blir svårare - fler och fler alger dyker upp
- Havsbotten-bakgrund med bubblor

### Mina instruktioner

#### Grundidén

Jag sa till Claude:

> Först ska det växa upp snabbt lite alger och sen ska de åka ner igen, och man ska försöka trycka på dem och så försvinner dem.

#### AIs följdfrågor och mina svar

Claude ställde frågor, och jag svarade:

- **Var ska algerna växa ifrån?** - På alla möjliga olika ställen
- **Hur ska algerna se ut?** - Som vanliga alger, som sjögräs
- **Hur snabbt åker de ner igen?** - Man ska hinna se dem ett tag
- **Vad händer när man trycker på en alg?** - Det ska vara en explosion som man ser och så hör man det. Det ska också låta när de åker upp och ner, eeeoo upp och ner
- **Ska man få poäng?** - Ja
- **Kommer det fler och fler alger?** - Ja det ska komma fler och fler
- **Ska spelet ha en bakgrund?** - Havsbotten

Sen la jag till:

> Det ska också vara två spelare

Claude ställde fler frågor:

- **Två spelare på samma skärm?** - Halva skärmen var, en röd linje i mitten
- **Hur vet man vem som tryckte?** - Olika färger och olika sidor
- **Hur länge pågår spelet?** - Den som först får 30
- **Vem vinner?** - Den som först får 30
- **Ska det finnas en startskärm?** - Börja direkt

### Hur mina instruktioner blev till kod

Här är vad Claude gjorde för att mina instruktioner skulle bli verklighet:

#### 1. Skapa havsbotten

Bakgrunden är en gradient som går från mörkt blå högst upp (vattnet) ner till brunt längst ner (havsbotten). Det finns också små bubblor som stiger uppåt för att det ska känna mer som under vattnet.

#### 2. Få alger att växa

Varje alg är en grön stam som växer uppåt med små blad på sidan - precis som sjögräs. De dyker upp på slumpmässiga ställen, växer upp, stannar kvar ett tag, och krymper sedan tillbaka ner. De vajar lite fram och tillbaka för att känna mer levande.

#### 3. Ljuden - eeeoo

Jag ville att det skulle låta "eeeoo" när algerna åker upp och ner. Claude använde Web Audio API för att skapa en ton som glider uppåt (eee) när algen växer och nedåt (ooo) när den krymper. När man träffar en alg hörs ett explosionsljud (vitt brus som tynar bort snabbt).

#### 4. Två spelare

Skärmen är delad på mitten med en röd linje. Spelare 1 (blå) spelar på vänster sida och spelare 2 (orange) spelar på höger sida. Alger dyker upp på båda sidor och varje spelare kan bara trycka på alger på sin egen sida.

#### 5. Poäng och vinst

Varje gång man trycker på en alg får man ett poäng och poängen studsar till lite för att det ska kännas bra. Den som först når 30 poäng vinner och då visas en vinnarskärm med en "Spela igen"-knapp.

#### 6. Svårare och svårare

I början dyker det upp en ny alg ungefär varannan sekund. Var femte sekund ökar takten så att alger dyker upp oftare och oftare. Till slut kommer de så snabbt att det är riktigt svårt att hinna med!

---

## :gb: English

A two-player game where seaweed grows up from the ocean floor and you have to tap it before it disappears!

Built with HTML, CSS and JavaScript using Claude Opus 4.6 (claude-opus-4-6) via Claude Code. No framework needed.

### Features

- Seaweed that grows up from the ocean floor in random places
- Two players on a split screen with a red line in the middle
- Explosion with sound when you hit a seaweed
- "Eeeoo" sound when seaweed grows up and down
- First player to 30 points wins
- It gets harder - more and more seaweed appears
- Ocean floor background with bubbles

### My instructions

#### The basic idea

I told Claude:

> First some seaweed should grow up quickly and then go back down again, and you should try to tap them and then they disappear.

#### The AI's follow-up questions and my answers

Claude asked questions, and I answered:

- **Where should the seaweed grow from?** - In all sorts of different places
- **What should the seaweed look like?** - Like regular seaweed, like sea grass
- **How fast do they go back down?** - You should have time to see them for a while
- **What happens when you tap a seaweed?** - There should be an explosion that you see and you hear it. It should also make a sound when they go up and down, eeeoo up and down
- **Should you get points?** - Yes
- **Do more and more seaweed appear?** - Yes, more and more should come
- **Should the game have a background?** - Ocean floor

Then I added:

> There should also be two players

Claude asked more questions:

- **Two players on the same screen?** - Half the screen each, a red line in the middle
- **How do you know who tapped?** - Different colors and different sides
- **How long does the game last?** - The one who first gets 30
- **Who wins?** - The one who first gets 30
- **Should there be a start screen?** - Start immediately

### How my instructions became code

Here is what Claude did to make my instructions become reality:

#### 1. Create the ocean floor

The background is a gradient that goes from dark blue at the top (the water) down to brown at the bottom (the ocean floor). There are also small bubbles rising upwards to make it feel more like being underwater.

#### 2. Make seaweed grow

Each seaweed is a green stem that grows upward with small leaves on the side - just like sea grass. They appear in random places, grow up, stay for a while, and then shrink back down. They sway slightly back and forth to feel more alive.

#### 3. The sounds - eeeoo

I wanted it to sound "eeeoo" when the seaweed goes up and down. Claude used the Web Audio API to create a tone that slides upward (eee) when the seaweed grows and downward (ooo) when it shrinks. When you hit a seaweed, an explosion sound plays (white noise that fades quickly).

#### 4. Two players

The screen is split in the middle with a red line. Player 1 (blue) plays on the left side and Player 2 (orange) plays on the right side. Seaweed appears on both sides and each player can only tap seaweed on their own side.

#### 5. Points and winning

Every time you tap a seaweed you get a point and the score bounces a little to make it feel good. The first player to reach 30 points wins and a winner screen is shown with a "Play again" button.

#### 6. Harder and harder

In the beginning, a new seaweed appears roughly every two seconds. Every five seconds the pace increases so that seaweed appears more and more frequently. Eventually they come so fast that it's really hard to keep up!
