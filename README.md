# 🌀 NEON VORTEX - A WebGL Demoscene Experience

A stunning interactive demoscene production built with WebGL, featuring real-time particle physics, synchronized audio generation, and dynamic visual effects powered by mouse interaction.

## ✨ Features

### Visual Effects
- **8000+ Main Particles**: Realistic black hole accretion physics with swirling motion
- **1500 Orbiting Particles**: Multiple orbital rings rotating around the central vortex
- **Geometric Structures**: 60 rotating geometric lines that pulse with the beat
- **Dynamic Lighting**: Color-shifting particles that change based on proximity to center
- **Beat Synchronization**: All visuals respond to the 120 BPM musical beat
- **Mouse Interaction**: Move your cursor to repel particles and create interactive effects

### Audio System
- **Complete Soundtrack**: 32-second loop with multiple synchronized layers
- **Drum Elements**:
  - Powerful kick drum with dynamic pitch sweep
  - Snare hits on backbeats
  - Hi-hat patterns for groove
  - Reverse bass for dramatic effect
  
- **Melodic Layers**:
  - Driving bassline following a pattern
  - Deep sub-bass for low-end punch
  - Energetic lead melody in the upper registers
  - Harmonic pads for richness
  - Shimmering high notes for texture
  - Spacey laser synth for atmosphere

- **Beat Timing**: 120 BPM with 64-beat loop structure for rich progression

### Interactive Elements
- **Mouse-Driven Particle Control**: Hover your mouse to push particles away
- **Influence Radius**: Effect strength decreases with distance from cursor
- **Real-time Response**: Instant visual feedback to mouse movement
- **Full-Screen Experience**: Responsive canvas that adapts to window size

## 🎮 How to Use

1. **Open the Demo**
   - Open `demo.html` in a modern web browser
   - Wait for the page to load (no external dependencies required)

2. **Enable Audio**
   - Click anywhere on the screen to unmute and start the synchronized audio
   - The music will begin playing with the full production soundtrack

3. **Interact with Particles**
   - Move your mouse cursor across the screen
   - Watch particles repel away from your cursor
   - Try moving your mouse quickly to create wave effects
   - The geometric lines and orbiting particles also respond to mouse movement

4. **Enjoy the Experience**
   - Let the demo run for ~30 seconds to see the credits appear
   - The entire production is synchronized - visuals match the music

## 🛠️ Technical Details

### WebGL Implementation
- **Shader System**: Custom vertex and fragment shaders for efficient particle rendering
- **Matrix Transformations**: Perspective projection, view matrices, and model transformations
- **Buffer Management**: Dynamic buffer updates for smooth real-time particle updates

### Physics Simulation
- **Gravity**: Central black hole attraction with squared distance falloff
- **Angular Momentum**: Swirling motion around the vortex
- **Friction**: Increased friction near the center (event horizon effect)
- **Turbulence**: Slight random motion for organic movement

### Audio Processing
- **Web Audio API**: Native browser audio synthesis
- **Oscillators**: Multiple waveforms (sine, triangle) for rich sound
- **Envelopes**: Attack, sustain, and release for musical expression
- **Filters**: Low-pass and high-pass filters for tone shaping

### Browser Compatibility
- Requires WebGL support (all modern browsers)
- Works best in Chrome, Firefox, Safari, and Edge
- Responsive to different screen sizes and resolutions

## 📊 Performance

- **Efficient Particle System**: 10,000+ particles running at 60 FPS
- **Optimized Rendering**: Point-based particle rendering for maximum performance
- **Real-time Updates**: Smooth animation with no frame drops
- **Low Latency**: Immediate response to mouse input

## 🎨 Customization

You can modify several aspects of the demo:

### Colors and Appearance
- Adjust the background gradient in the CSS `#canvas` style
- Modify particle color ranges in the `generateParticles()` function
- Change the glow effects in the CSS

### Audio
- Modify BPM in `generateMusic()` (currently 120)
- Adjust beat patterns in the `bassLine` array
- Change frequencies and durations in note generation
- Tweak volumes in `playNote()` function calls

### Particle Physics
- `gravityStrength`: Controls black hole pull (line ~630)
- `angularForce`: Controls swirling motion (line ~642)
- `mouseInfluenceRange`: Controls mouse interaction distance
- `particleCount`: Number of particles to simulate

### Visual Effects
- Camera movement controlled by `elapsed` in the `createViewMatrix()` call
- Model rotation speeds in `rotateMatrix()` calls
- Point size in vertex shader (currently 15.0)

## 🚀 Requirements

- **Modern Web Browser** with WebGL support
- **HTML5** and **JavaScript ES6**
- No external libraries or dependencies
- No internet connection required (fully self-contained)

## 📝 Notes

- The demo uses the **Web Audio API** for sound synthesis
- All graphics are rendered with **WebGL** for smooth performance
- The experience is best viewed in **fullscreen**
- Audio context requires user interaction (click to unmute) due to browser autoplay policies
- The demo loops continuously with credits appearing after ~30 seconds

## 🎬 Credits

**NEON VORTEX** - A Demoscene Production for 2026
Pure WebGL Magic

---

Enjoy the experience! Move your mouse to interact with the particles and let the synchronized audio and visuals transport you to another dimension. 🌌✨
