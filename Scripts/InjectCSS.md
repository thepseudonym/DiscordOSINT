# Inject CSS
```js
const injectCss = (id, css) => {
  const style = document.createElement('style');
  style.id = id;
  style.innerText = css;
  document.head.appendChild(style);
  return style;
}
```

# Inject big CSS
I couldn't find any javascript code for the moment. <br>
You can use [BeautifulDiscord](https://github.com/leovoel/BeautifulDiscord) or [BetterDiscord](https://betterdiscord.app).<br>
If you don't need discord plugins, I recommend [BeautifulDiscord](https://github.com/leovoel/BeautifulDiscord).

___	

## Text shadow
```js
injectCss('nashy_TextShadow', `
.cozy-3raOZG .header-23xsNx,
.markup-2BOw-j {
    color: white;
    text-shadow: 4px 4px 5px black,2px 3px 5px black;
}
`);
```
## Message slide
```js
injectCss('nashy_Slide', `
@keyframes slide-up {
    0% {
        opacity: 0;
        transform: translateX(20px);
    }
    100% {
        opacity: 1;
        transform: translateX(0);
    }
}
.message-2qnXI6 {
  animation: slide-up 0.4s ease;
}
`);
```

## Change base color (default: blurple).
<details>
<summary></summary>

```js
injectCss('nashy_customBlurple', `
.theme-dark, .theme-light {
  --color: 255, 102, 102;

	--info-help-text: #fff;
	--control-brand-foreground: rgb(var(--color)) !important;
	--control-brand-foreground-new: rgb(var(--color)) !important;
	--brand-experiment-100: #fdfdfd !important;
	--brand-experiment-130: #f2f2f2 !important;
	--brand-experiment-160: #ebebeb !important;
	--brand-experiment-200: #e3e3e3 !important;
	--brand-experiment-230: #dadada !important;
	--brand-experiment-260: #d1d1d1 !important;
	--brand-experiment-300: #c7c7c7 !important;
	--brand-experiment-330: rgb(var(--color)) !important;
	--brand-experiment-360: rgb(var(--color)) !important;
	--brand-experiment-400: rgb(var(--color)) !important;
	--brand-experiment-430: rgb(var(--color)) !important;
	--brand-experiment-460: rgb(var(--color)) !important;
	--brand-experiment: rgb(var(--color)) !important;
	--brand-experiment-500: rgb(var(--color)) !important;
	--brand-experiment-530: rgb(var(--color)) !important;
	--brand-experiment-560: rgb(var(--color)) !important;
	--brand-experiment-600: rgb(var(--color)) !important;
	--brand-experiment-630: rgb(var(--color)) !important;
	--brand-experiment-660: rgb(var(--color)) !important;
	--brand-experiment-700: #323232 !important;
	--brand-experiment-730: #2b2b2b !important;
	--brand-experiment-760: #272727 !important;
	--brand-experiment-800: #222222 !important;
	--brand-experiment-830: #1a1a1a !important;
	--brand-experiment-860: #111111 !important;
	--brand-experiment-900: #0b0b0b !important;
	--brand-experiment-05a: rgba(var(--color),.05) !important;
	--brand-experiment-10a: rgba(var(--color),.1) !important;
	--brand-experiment-15a: rgba(var(--color),.15) !important;
	--brand-experiment-20a: rgba(var(--color),.2) !important;
	--brand-experiment-25a: rgba(var(--color),.25) !important;
	--brand-experiment-30a: rgba(var(--color),.3) !important;
	--brand-experiment-35a: rgba(var(--color),.35) !important;
	--brand-experiment-40a: rgba(var(--color),.4) !important;
	--brand-experiment-45a: rgba(var(--color),.45) !important;
	--brand-experiment-50a: rgba(var(--color),.5) !important;
	--brand-experiment-55a: rgba(var(--color),.55) !important;
	--brand-experiment-60a: rgba(var(--color),.6) !important;
	--brand-experiment-65a: rgba(var(--color),.65) !important;
	--brand-experiment-70a: rgba(var(--color),.7) !important;
	--brand-experiment-75a: rgba(var(--color),.75) !important;
	--brand-experiment-80a: rgba(var(--color),.8) !important;
	--brand-experiment-85a: rgba(var(--color),.85) !important;
	--brand-experiment-90a: rgba(var(--color),.9) !important;
	--brand-experiment-95a: rgba(var(--color),.95) !important;
}
`);
```

credit: [BlurpleRecolor theme](https://mwittrien.github.io/BetterDiscordAddons/Themes/BlurpleRecolor/BlurpleRecolor.css) 
