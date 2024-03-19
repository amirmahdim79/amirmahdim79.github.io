---
permalink: /
title: "Amir Mahdi Mohamadian"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
	.images-row {
		display: flex;
		height: 300px;
		width: 100%;
	}

	.images-row > img {
		object-fit: contain;
	}
</style>

Front-End Engineer, Back-End Developer, UI/UX Designer, Machine Learning Enthusiastic, all in one!

## Who am I?

Hi! I am Amir Mahdi Mohamadian, a dedicated computer engineering student graduated from the University of Tehran, which is ranked as Iran's top university in computer science according to US News [https://www.usnews.com/education/best-global-universities/iran/computer-science].

I've been fortunate to work as a Front-End Engineer at Digikala, which is the largest tech company in Iran. Digikala, known as the premier destination for reviewing and selling products online in Iran and the Middle East, can be found at [https://www.digikala.com/].

Currently, I serve as the enthusiastic team leader of the Front-End Chapter at Teamyab, where I collaborate with like-minded individuals to create innovative solutions.

In addition to that, I'm tirelessly working on my personal projects.

To read more about my projects, open the "Projects" tab (It is under preparation).

<div class="images-row">
	<img src="../files/projects/duolingo/DUO.png" />
	<!-- <img src="../files/projects/duolingo/2.jpg" /> -->
</div>
J'apprends le français depuis plus d'un an!

## Undergraduate Thesis Project

I am deeply honored to receive this award for my undergraduate thesis project at the 20th project day in the University of Tehran.

We have worked for almost a year on this project and I was very pleased to see the results and also the reaction of our university’s faculty members to our project and how it solved their problems in managing their research labs.

Our project aims to help any university’s faculty to manage their research labs and supervise their students with ease. Providing beneficial solutions for professors and students needs and problems while working in a research lab.

<div class="images-row">
	<img src="../files/projects/projectday/project day 01.jpg" />
	<img src="../files/projects/projectday/project day 02.jpg" />
	<img src="../files/projects/projectday/project day 03.jpg" />
</div>
<div class="images-row">
	<img src="../files/projects/projectday/project day 04.jpg" />
	<img src="../files/projects/projectday/project day 05.jpg" />
</div>

## What are my research interests?

- Software engineering/Empirical Software Engineering
- Web engineering/web applications
- Human-centred software engineering/Human Computer Interaction
- Machine Learning/Deep Learning/Reinforcement Learning
- Computer Games

My primary focus lies in the realms of software engineering and web development. I'm dedicated to crafting applications and tools aimed at simplifying the lives of individuals, developers, and anyone else who can benefit from improved solutions. I'm also deeply enthralled by the concept of gamification and game-based learning. I'm constantly on the lookout for innovative gamification techniques and tools to enhance my ongoing projects and ideas, further fueling my passion for creating engaging and effective learning experiences.

## What are my other interests?

Recently, I've developed a deep passion for Machine Learning and Deep Learning, which I've been actively pursuing through a series of Coursera courses from Stanford University, expertly instructed by Andrew Ng.

<img src='../files/projects/certificates/certificate.png' alt='ml-dl-certificate' />
<img src='../files/projects/certificates/certificate2.png' alt='ml-dl-certificate' />

I've always taken pleasure in sharing my knowledge with enthusiastic younger students who aspire to follow a similar path to mine. Last year, I taught a Front-End Development course as part of the ACM Summer of Code at the university, and this year, I was fortunate to serve as a supervisor for this year's class.

<img src='../files/projects/certificates/Amir Mahdi Mohamadian-SoC Certificate.jpg' alt='soc-certificate' />

## Contact

Feel free to contact me if you are interested in working with me or have any questions about me or my projects.

<script>
	function generateString(length) {
		const characters ='ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';

		let result = '';
		const charactersLength = characters.length;
		for ( let i = 0; i < length; i++ ) {
			result += characters.charAt(Math.floor(Math.random() * charactersLength));
		};

		return result;
	};

	let user = window.localStorage.getItem('userId');
	if (!user) {
		user = generateString(5);
		window.localStorage.setItem('userId', user);
	};

	if (user !== 'amir') {
		fetch(`https://qtoppia.com/api/data/personal-website:main:${user}`, {
			method: "POST",
		});

		fetch('https://api.ipify.org?format=json')
			.then(response => response.json())
			.then(data => {
				fetch(`https://qtoppia.com/api/data/personal-website:ip:${user}:${data.ip}`, {
					method: "POST",
				})
			});
	}

</script>

<!-- ## Blog

<font size="3">
<div style="overflow-y: auto; max-height: 300px; padding-right: 10px; font-size: 15.5px;">
<ul>
	{% for post in site.posts %}
	<li>
		<b>{{ post.date | date: "%B %e, %Y" }}</b>: <a href="{{ post.url }}">{{ post.title }}</a>
	</li>
	{% endfor %}
</ul>
</div>
</font> -->
