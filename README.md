# REALLY-HI-HAT

a web audio hi-hat synth, inspired by [Synthesizing Hi-Hats with Web Audio by Joe Sullivan](http://joesul.li/van/synthesizing-hi-hats/)





# USE IT
var rhh = require('really-hi-hat')(yrAudioContext)
rhh.start(yrAudioContext.currentTime)
rhh.update({peak: 0.5})
rhh.start(yrAudioContext.currentTime + 1)

# settings for the update settings
```
settings: {
  attack: 0.02,
  decay: 0.03,
  sustain: 0.000001,
  release: 0.3,
  peak: 0.7,
  mid: 0.25,
  end: 0.00001
}

```






# DEVELOPMENT

```
npm install
npm run test # should pass! Yay!
```

# HEAR THE MAGIC!

- `npm run serve` boot a webserver at port 3000
- `npm run build` build demo.js to a bundle. Run this after making any changes to hear updates (or add [watchify](https://github.com/wham-js/web-audio-advent-calendar/blob/master/package.json#L8), i wanted to keep things "light")
- open `http://localhost:3000/` in a web browser and hear the magic (hopefully)

# RESOURCES


- [openmusic](https://github.com/openmusic) has a ton of helpful modules
- if you need a basic convolver impulse, [voila](https://github.com/mdn/voice-change-o-matic/tree/gh-pages/audio)