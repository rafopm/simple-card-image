# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - NFT preview card component solution](#frontend-mentor---nft-preview-card-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Screenshot](https://github.com/rafopm/simple-card-image/blob/main/public/images/captura-nft-preview-card-component-challenge.jpg?raw=true)


### Links

- Solution URL: [https://github.com/rafopm/simple-card-image/blob/main/src/components/card.astro](https://github.com/rafopm/simple-card-image/blob/main/src/components/card.astro)
- Live Site URL: [https://nft-preview-card-component-challenge.netlify.app/](https://nft-preview-card-component-challenge.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- [Astro](https://astro.build/)


### What I learned

Overlay on image


```html
<div class="img-container">
				<img
					src="/images/image-equilibrium.jpg"
					class="card-img"
					alt=""
				/>
				<div class="overlay">
					<img src="/images/icon-view.svg" alt="View" />
				</div>
			</div>
```
```css
.card .img-container {
		position: relative;
		align-self: center;
		margin: 20px;
		width: 280px;
		height: 280px;
		border-radius: 5px;
	}

	.card .card-img {
		width: 100%;
		height: 100%;
		border-radius: 5px;
	}

	.card .overlay {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background-color: rgba(0, 255, 255, 0.5);
		border-radius: 5px;
		display: none;
		place-items: center;
		justify-content: center;
	}

	.card .img-container:hover {
		cursor: pointer;
	}

	.card .img-container:hover .overlay {
		display: grid;
	}
```


### Continued development

I am a full stack developer but at the moment I am focused on developing frontend skills.

## Author

- Website - [Add your name here](https://rafopm.netlify.app/)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/rafopm)
