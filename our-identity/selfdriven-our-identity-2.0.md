# Colours

> Colour names based on "Name That Color (Chirag Mehta)"

| Chirag Mehta Name | Color Name | Hex Code  |
|-------------------|------------|-----------|
| [White](#white-white) | White | #FFFFFF |
| [Cararra](#cararra-beige) | Beige | #EFEFE5 |
| [Melrose](#melrose-light-purple) | Light Purple | #B4A1FB |
| [Blackcurrant](#blackcurrant-dark-purple) | Dark Purple | #420633 |
| [Flamingo](#flamingo-orange) | Orange | #DE5A31 |
| [Black](#black-black) | Black | #000000 |

## White (White)
**White is the brightest and most neutral color. It’s used as a background, highlight, or contrast color in almost all design systems. In your palette, it serves best as: light mode background, highlight text on dark backgrounds & borders, shadows, or accents in minimal UI.**
- Category: Pure white
- Hex: #FFFFFF
- RGB: rgb(255, 255, 255)
- HSL: hsl(0°, 0%, 100%)
- Background: #FFFFFF;
- Text: background: linear-gradient(356.15deg, #420633 4.27%, rgba(66, 6, 51, 0.5) 202.17%);

```css
:root {
  --color-white: #FFFFFF; /* White - Pure neutral highlight or background */
}
.theme-dark {
  --color-white: #F0F0F0;        /* Optional: softer white for reduced glare */
  --color-white-pure: #FFFFFF;   /* Reserved for high contrast when needed */
}
```

## Cararra (Beige)
**Cararra is a very light, slightly warm off-white with a subtle yellow-green tint. It’s ideal for backgrounds where you want a touch of warmth without losing that clean, bright feel. Often used in minimal or soft aesthetic palettes.**

- Category: Pale neutral / off-white
- Hex: #EFEFE5
- RGB: rgb(239, 239, 229)
- HSL: hsl(60°, 26%, 92%)
- Background: #EFEFE5;
- Text: background: linear-gradient(356.15deg, #420633 4.27%, rgba(66, 6, 51, 0.5) 202.17%);

| Role              | Color Name       | Hex Code  | Description                                   |
|-------------------|------------------|-----------|-----------------------------------------------|
| **Primary**       | Cararra          | `#EFEFE5` | Warm, pale off-white with slight green-yellow |
| **Complement**    | Slate Gray       | `#708090` | Muted blue-gray for contrast                  |
| **Accent**        | Burnt Sienna     | `#E97451` | Warm earthy orange-red                        |
| **Soft Contrast** | Dusty Mauve      | `#BFAFB2` | Subtle contrast with elegant undertone        |
| **Neutral Light** | Spring Wood      | `#F5F5ED` | Near-white for light backgrounds              |
| **Neutral Dark**  | Graphite         | `#2F2F2F` | Deep gray for dark text or UI elements        |
| **Highlight**     | White            | `#FFFFFF` | Clean highlight for borders or emphasis       |

```css
:root {
  --color-primary:         #EFEFE5; /* Cararra - Warm, pale off-white */
  --color-secondary:       #708090; /* Slate Gray - Muted blue-gray for contrast */
  --color-accent:          #E97451; /* Burnt Sienna - Warm earthy orange-red */
  --color-neutral-light:   #F5F5ED; /* Spring Wood - Near-white for soft backgrounds */
  --color-neutral-dark:    #2F2F2F; /* Graphite - Deep neutral for text/UI anchors */
  --color-contrast:        #BFAFB2; /* Dusty Mauve - Elegant soft contrast */
  --color-highlight:       #FFFFFF; /* White - Crisp highlight */
}

.theme-dark {
  --color-primary:         #2A2A2A; /* Cararra adapted for dark mode base */
  --color-secondary:       #8A9BAA; /* Lightened Slate Gray */
  --color-accent:          #FF8866; /* Brighter Burnt Sienna for energy */
  --color-neutral-light:   #1E1E1E; /* Deeper background panel tone */
  --color-neutral-light-2: #121212; /* Very deep black for surfaces */
  --color-neutral-dark:    #D0C5C8; /* Lighter mauve for headings/elements */
  --color-contrast:        #F0F0F0; /* Light gray text */
  --color-highlight:       #FFFFFF; /* White - for max contrast where needed */
}
```

## Melrose (Light Purple)
**Melrose is a gentle, light violet with a cool blue undertone — often associated with calm, creativity, and softness. It pairs nicely with whites, lavenders, and muted golds or warm neutrals.**

- background: #B4A1FB;
- text: background: linear-gradient(356.15deg, #420633 4.27%, rgba(66, 6, 51, 0.5) 202.17%);
- Hex: #B4A1FB
- RGB: rgb(180, 161, 251)
- HSL: hsl(252°, 93%, 81%)
- Category: Soft pastel purple / periwinkle

| Role              | Color Name      | Hex Code  | Description                            |
|-------------------|------------------|-----------|----------------------------------------|
| **Primary**       | Melrose          | `#B4A1FB` | Soft pastel purple                     |
| **Secondary**     | Lavender Blue    | `#C3B6FD` | Lighter complementary tone             |
| **Accent**        | Flamingo         | `#DE5A31` | Warm orange-red contrast               |
| **Neutral Light** | Spring Wood      | `#F0EFE4` | Subtle off-white                       |
| **Neutral Dark**  | Blackcurrant     | `#420633` | Deep purple anchor                     |
| **Contrast**      | Charcoal         | `#333333` | Strong neutral for text                |
| **Highlight**     | Mint Cream       | `#F5FFFA` | Cool highlight white                   |


```css
:root {
  --color-primary:       #B4A1FB; /* Melrose - Soft pastel purple */
  --color-secondary:     #C3B6FD; /* Lavender Blue - Lighter complementary tone */
  --color-accent:        #DE5A31; /* Flamingo - Warm orange-red contrast */
  --color-neutral-light: #F0EFE4; /* Spring Wood - Subtle off-white */
  --color-neutral-dark:  #420633; /* Blackcurrant - Deep purple anchor */
  --color-contrast:      #333333; /* Charcoal - Strong neutral for text */
  --color-highlight:     #F5FFFA; /* Mint Cream - Cool highlight white */
}

.theme-dark {
  --color-primary:         #B4A1FB; /* Melrose - still vibrant on dark */
  --color-secondary:       #9A85E0; /* Darker Lavender Blue */
  --color-accent:          #FF7A4D; /* Brighter Flamingo for strong contrast */
  --color-neutral-light:   #2C2C2C; /* Dark gray for background */
  --color-neutral-light-2: #1F1F1F; /* Even deeper background or panel tone */
  --color-neutral-dark:    #D3B1DC; /* Lightened plum for UI text/accent */
  --color-contrast:        #F0F0F0; /* Light gray for main text */
  --color-highlight:       #FFFFFF; /* White for sharp text or borders */
}
```



## Blackcurrant (Dark Purple)
**“Blackcurrant” is a very dark, rich purple with strong red undertones — bold, moody, and great as an accent or background when you want depth or luxury. It’s commonly used in fashion, premium branding, and gothic/vintage palettes.**

- Category: Deep purple / dark magenta
- Background: linear-gradient(356.27deg, #420633 4.18%, rgba(66, 6, 51, 0.75) 97.03%);
- Text: background: linear-gradient(356.15deg, #420633 4.27%, rgba(66, 6, 51, 0.5) 202.17%);
- Hex: #420633
- RGB: rgb(66, 6, 51)
- HSL: hsl(318°, 84%, 14%)

| Role              | Color Name       | Hex Code  | Description                                      |
|-------------------|------------------|-----------|--------------------------------------------------|
| **Primary**       | Blackcurrant     | `#420633` | Deep, rich purple with red undertones           |
| **Complement**    | Soft Lime        | `#C1FB9D` | Pale green contrast for vibrancy                 |
| **Accent**        | Orchid           | `#DA70D6` | Bright pink-purple for energy                    |
| **Analogous 1**   | Plum             | `#580F41` | Slightly redder purple for harmony               |
| **Analogous 2**   | Midnight Purple  | `#2A0030` | Darker purple tone for depth                     |
| **Neutral Light** | Spring Wood      | `#F0EFE4` | Soft off-white to balance richness               |
| **Neutral Dark**  | Raisin Black     | `#23101A` | Very dark muted tone to complement darkness      |
| **Highlight**     | Lavender Mist    | `#EDE1F9` | Light, airy purple for text or soft backgrounds  |


```css
:root {
  --color-primary:            #420633; /* Blackcurrant - Deep, rich purple */
  --color-complement:         #C1FB9D; /* Soft Lime - Pale green contrast */
  --color-accent:             #DA70D6; /* Orchid - Vibrant pink-purple */
  --color-analogous-1:        #580F41; /* Plum - Warmer purple tone */
  --color-analogous-2:        #2A0030; /* Midnight Purple - Darker variation */
  --color-neutral-light:      #F0EFE4; /* Spring Wood - Soft off-white */
  --color-neutral-dark:       #23101A; /* Raisin Black - Very dark base */
  --color-highlight:          #EDE1F9; /* Lavender Mist - Light pastel highlight */
}
.theme-dark {
  --color-primary:            #C27BD4; /* Lightened Blackcurrant for visibility on dark */
  --color-complement:         #A4FF89; /* Brighter lime green */
  --color-accent:             #FF9AED; /* Electric pink-purple */
  --color-analogous-1:        #7A2E60; /* Medium plum */
  --color-analogous-2:        #3A0A49; /* Softer midnight purple */
  --color-neutral-light:      #1F1A1B; /* Dark neutral background */
  --color-neutral-dark:       #0F0C0E; /* Very deep gray */
  --color-highlight:          #F6EDFC; /* Lavender-tinged white */
}
```


## Flamingo (Orange)
**Flamingo is a vibrant, warm-toned orange with a hint of red — energetic and bold. It gives a retro, summery feel and works well in playful or attention-grabbing designs.**

- Category: Warm orange-red
- Hex: #DE5A31
- RGB: rgb(222, 90, 49)
- HSL: hsl(15°, 74%, 53%)
- Background: #DE5A31;
- Text: background: linear-gradient(356.15deg, #420633 4.27%, rgba(66, 6, 51, 0.5) 202.17%);

| Role              | Color Name       | Hex Code  | Description                              |
|-------------------|------------------|-----------|------------------------------------------|
| **Primary**       | Flamingo         | `#DE5A31` | Bold, warm orange-red                    |
| **Complement**    | Denim Blue       | `#3170DE` | Cool blue for strong contrast            |
| **Analogous 1**   | Coral            | `#DE8A31` | Orange-leaning version for warmth        |
| **Analogous 2**   | Rose Red         | `#DE3152` | Redder side of the Flamingo hue          |
| **Neutral Light** | Spring Wood      | `#F0EFE4` | Soft off-white for background            |
| **Neutral Dark**  | Charcoal         | `#333333` | Deep neutral for text or balance         |
| **Highlight**     | White            | `#FFFFFF` | Clean, crisp white for text or borders   |


```css
:root {
  --color-primary:         #DE5A31; /* Flamingo - Bold, warm orange-red */
  --color-complement:      #3170DE; /* Denim Blue - Cool contrast */
  --color-analogous-1:     #DE8A31; /* Coral - Orange side */
  --color-analogous-2:     #DE3152; /* Rose Red - Reddish tone */
  --color-neutral-light:   #F0EFE4; /* Spring Wood - Soft off-white */
  --color-neutral-dark:    #333333; /* Charcoal - Strong dark neutral */
  --color-highlight:       #FFFFFF; /* White - For text or borders */
}

.theme-dark {
  --color-primary:         #FF6A3D; /* Brighter version of Flamingo for pop on dark */
  --color-complement:      #4A90E2; /* Slightly lighter denim blue for contrast */
  --color-analogous-1:     #FF944D; /* Warm coral - keeps vibrancy in dark mode */
  --color-analogous-2:     #FF4D68; /* Bright rose-red tone */
  --color-neutral-light:   #2A2A2A; /* Dark gray background */
  --color-neutral-dark:    #1A1A1A; /* Deeper surface (e.g., cards/panels) */
  --color-contrast:        #F0F0F0; /* Main text color */
  --color-highlight:       #FFFFFF; /* Sharp accents/highlights */
}
```


## Black (Black)
**Black is the deepest shade, used for maximum contrast. It’s great for: Text on light backgrounds, Accents, outlines, or shadows Neutral anchor for balancing vivid palettes**

- Category: Pure black
- Hex: #000000
- RGB: rgb(0, 0, 0)
- HSL: hsl(0°, 0%, 0%)
- Background: #000000;
- Text: background: linear-gradient(191.23deg, #A474C0 29.32%, #752A62 105.03%);


```css
:root {
  --color-black:       #000000; /* Pure Black - for strong text or accents */
}

.theme-dark {
  --color-black:           #121212; /* Default soft black for base background */
  --color-black-soft:      #1A1A1A; /* Softer variant for surfaces */
}
```


# Fonts

## Brockman (Logos)
https://www.atipofoundry.com/fonts/brockmann

- font-family: Brockmann;
- font-weight: 500;
- font-size: 215px;
- line-height: 100%;
- letter-spacing: -5%;
- text-align: center;

## Poppins (Everything by Logos)
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
```

```css
/* poppins-100 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 100;
  src: url('../fonts/poppins-v23-latin-100.woff2') format('woff2');
}

/* poppins-100italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 100;
  src: url('../fonts/poppins-v23-latin-100italic.woff2') format('woff2');
}
/* poppins-200 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 200;
  src: url('../fonts/poppins-v23-latin-200.woff2') format('woff2');
}
/* poppins-200italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 200;
  src: url('../fonts/poppins-v23-latin-200italic.woff2') format('woff2');
}
/* poppins-300 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 300;
  src: url('../fonts/poppins-v23-latin-300.woff2') format('woff2');
}
/* poppins-300italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 300;
  src: url('../fonts/poppins-v23-latin-300italic.woff2') format('woff2');
}
/* poppins-regular - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 400;
  src: url('../fonts/poppins-v23-latin-regular.woff2') format('woff2');
}
/* poppins-italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 400;
  src: url('../fonts/poppins-v23-latin-italic.woff2') format('woff2');
}
/* poppins-500 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 500;
  src: url('../fonts/poppins-v23-latin-500.woff2') format('woff2');
}
/* poppins-500italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 500;
  src: url('../fonts/poppins-v23-latin-500italic.woff2') format('woff2');
}
/* poppins-600 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 600;
  src: url('../fonts/poppins-v23-latin-600.woff2') format('woff2');
}
/* poppins-600italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 600;
  src: url('../fonts/poppins-v23-latin-600italic.woff2') format('woff2');
}
/* poppins-700 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 700;
  src: url('../fonts/poppins-v23-latin-700.woff2') format('woff2');
}
/* poppins-700italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 700;
  src: url('../fonts/poppins-v23-latin-700italic.woff2') format('woff2');
}
/* poppins-800 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 800;
  src: url('../fonts/poppins-v23-latin-800.woff2') format('woff2');
}
/* poppins-800italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 800;
  src: url('../fonts/poppins-v23-latin-800italic.woff2') format('woff2');
}
/* poppins-900 - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 900;
  src: url('../fonts/poppins-v23-latin-900.woff2') format('woff2');
}
/* poppins-900italic - latin */
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: italic;
  font-weight: 900;
  src: url('../fonts/poppins-v23-latin-900italic.woff2') format('woff2');
}
```