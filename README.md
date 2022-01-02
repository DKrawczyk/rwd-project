Foto

Thanks for watching my first HTML and CSS RWD project! :)

You can see this website (link here). 
It is based on Colorlib free template.


# Installation

This project doesn't use node or npm. This website is made by pure HTML and CSS.


# Solutions provided in the project

- To achieve this result I used Perfect Pixel and ColorZilla web extension

- I used basic reset CSS for better and easier styling without not necessary margins and other problems 

- My first animated hamburger icon 

	.hamburger::before, .hamburger::after {
		content: '';
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		border-top: 5px solid #ffffff;
		transform: translateY(5px);
	}

	.hamburger::after {
		transform: translateY(15px);
		transition: 0.3s transform linear;
	}

	input:checked + .hamburger {
		transform: rotate(45deg) translateY(10px); 
		border: none;
	}

	input:checked + .hamburger::after {
		transform: rotate(-90deg) translateX(-5px);
	}

- Made hamburger icon without using JavaScript, just pure HTML and CSS using input and checkbox technic

		<input type="checkbox" id="menu-switcher" class="menu__switcher"/>
        <label class="hamburger" for="menu-switcher" ></label>


	input:checked + .hamburger + .navigation__list {
		display: block;
	}

	input:checked + .hamburger {
		transform: rotate(45deg) translateY(10px); 
		border: none;
	}

- Used https://gs.statcounter.com/ website to check and decide, which resolution is the best to support most devices

- This project is a fully responsive landing page made for phones, tablets and desktop version

- In this project I tried to use the BEM methodology

- This project includes global.css to prevent writing unnecessary code, for example:

		:root {
		--color-alfa: white;
		--color-beta: black;
	}

- In this project I used CSS grid layout to make the website more readable and just for fun, to try my skills :)

- Font were imported from https://fonts.google.com/


# Conclusions for future solutions:

Next time if the project would have more than two columns I will use a grid layout. Otherwise, I think that flex is one of the best ways to style websites.
Every solution made without using webpack should be check in https://caniuse.com/ website and optimization solutions should be checked by https://search.google.com/test/mobile-friendly.

The next project would be a great opportunity to use SCSS and SASS technology. Functions like clamp(), calc() would be also a great idea to use in the next website.


# Special thanks
To my [mentor](https://github.com/devmentor-pl) for creating the task and for the code review!