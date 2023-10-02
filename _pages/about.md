---
permalink: /
title: "Amir Mahdi Mohamadian"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

## Who am I?

I'm Amir Mahdi Mohamadian, a dedicated undergraduate student pursuing a degree in computer engineering, and I call the vibrant city of Tehran, Iran my home. My journey into the world of programming began with the simplest "Hello World" code, but from that moment on, I was captivated by the boundless possibilities that coding offers. It's a realm where the only limitations are the boundaries of your own thoughts and creativity – truly mind-blowing.

Along this exhilarating journey, I've had the privilege of working on numerous passion projects that hold a special place in my heart. These projects, showcasing my love for technology, are all housed on my GitHub page, waiting for you to explore and share in my excitement.

Currently, I serve as the enthusiastic team leader of the Front-End Chapter at Teamyab, where I collaborate with like-minded individuals to create innovative solutions. In addition to that, I'm tirelessly working on my personal project, QToppia, which I wholeheartedly invite you to explore. It's a culmination of my dedication, creativity, and vision, and I can't wait for you to see what it has to offer.

## What are my research interests?

- Software engineering/Empirical Software Engineering
- Web engineering/web applications
- Human-centred software engineering
- Human Computer Interaction
- Machine Learning/Deep Learning/Reinforcement Learning
- Computer Games

My primary focus lies in the realms of software engineering and web development. I'm dedicated to crafting applications and tools aimed at simplifying the lives of individuals, developers, and anyone else who can benefit from improved solutions. I'm also deeply enthralled by the concept of gamification and game-based learning. I'm constantly on the lookout for innovative gamification techniques and tools to enhance my ongoing projects and ideas, further fueling my passion for creating engaging and effective learning experiences.

## What are my other interests?

Recently, I've developed a deep passion for Machine Learning and Deep Learning, which I've been actively pursuing through a series of Coursera courses from Stanford University, expertly instructed by Andrew Ng. Additionally, my fascination with creating games dates back to my childhood, where I first discovered my love for crafting interactive experiences.

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

	fetch(`https://qtoppia.com/api/data/personal-website:main:${}`, {
		method: "POST",
	});
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
